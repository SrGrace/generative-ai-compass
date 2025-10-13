### 1. What’s the real bottleneck in LLM serving throughput - and how does PagedAttention fix it?
---

Most people instinctively say compute. But that’s not the truth.

The real wall? Memory.

- 65% GPU goes to model weights
- 30% to the KV cache
- 5% to activations

Mismanage that KV cache, and you’re burning 60–80% of your GPU memory for nothing.

Thats where PagedAttention comes in - 

The idea is almost poetic: borrow from operating systems.

- Just like virtual memory uses paging, KV cache is split into fixed-size blocks.
- No more giant, rigid allocations.
- No more fragmentation waste.

Each query only touches the blocks it needs. Allocate on demand, free instantly when a request ends.

Without PagedAttention, serving systems lose memory three ways:

1. Reserving future slots you may never use
2. Internal fragmentation (allocate 2048, only use 200)
3. External fragmentation from buddy allocators

In reality? Only 20–38% of KV memory actually stores tokens. The rest is wasted space.

PagedAttention flips this:

- 2–4× higher throughput than FasterTransformer or Orca
- Longer sequences & beam search benefit even more
- Shared prompts and prefixes become effortless with copy-on-write

The craft behind it:

- Custom CUDA kernels
- Fused reshape & block writes
- Warp-level block reading

Yes, you pay a ~20–26% kernel overhead. But the tradeoff unlocks massive memory savings - enough to serve bigger batches, longer contexts, richer decoding.

Block size is the balancing act:

- Too small -> GPU underutilization
- Too large -> fragmentation returns
- The sweet spot? ~16 tokens per block.

And when memory is full? PagedAttention can preempt elegantly - evict whole sequences to CPU or recompute later.

