## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Chain-of-Thought Matters: Improving Long-Context Language Models with Reasoning Path Supervision](https://arxiv.org/pdf/2502.20790) | LLMs struggle with long-context reasoning. 🫠 <br><br> They can read thousands of tokens, but pulling the right information and reasoning through it? That’s where things fall apart. <br><br> So, I looked at why this happens. <br> &nbsp;  -> LLMs often retrieve the wrong information from long documents. <br> &nbsp;  -> Chain-of-Thought (CoT) helps, but not always - sometimes it adds unnecessary steps. <br> &nbsp;  -> Even when CoT works, models don’t learn how to reason better over time. <br><br> What’s the fix? 
This recent paper proposes LONGREPS - a process-supervised approach that teaches LLMs how to reason over long contexts. It -  <br> &nbsp;  -> Bootstraps reasoning paths by letting the model generate multiple solutions. <br> &nbsp;  -> Filters out low-quality reasoning using a new quality assessment method. <br> &nbsp;  -> Fine-tunes models on only high-quality reasoning paths to improve long-context understanding. <br><br> And the results? <br> &nbsp;  ✅ +13.6 F1 gain on MuSiQue, a multi-hop QA benchmark. <br> &nbsp;  ✅ +9.3 average improvement across multiple long-context reasoning tasks. <br> &nbsp;  ✅ Better generalization across domains like legal, finance, and academic research. | LLM Reasoning |
| []() |  |  |



## Week 2/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |



## Week 3/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |



## Week 4/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |
