## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Chain-of-Thought Matters: Improving Long-Context Language Models with Reasoning Path Supervision](https://arxiv.org/pdf/2502.20790) | LLMs struggle with long-context reasoning. 🫠 <br><br> They can read thousands of tokens, but pulling the right information and reasoning through it? That’s where things fall apart. <br><br> So, I looked at why this happens. <br> &nbsp;  -> LLMs often retrieve the wrong information from long documents. <br> &nbsp;  -> Chain-of-Thought (CoT) helps, but not always - sometimes it adds unnecessary steps. <br> &nbsp;  -> Even when CoT works, models don’t learn how to reason better over time. <br><br> What’s the fix?  <br><br> This recent paper proposes LONGREPS - a process-supervised approach that teaches LLMs how to reason over long contexts. It -  <br> &nbsp;  -> Bootstraps reasoning paths by letting the model generate multiple solutions. <br> &nbsp;  -> Filters out low-quality reasoning using a new quality assessment method. <br> &nbsp;  -> Fine-tunes models on only high-quality reasoning paths to improve long-context understanding. <br><br> And the results? <br> &nbsp;  ✅ +13.6 F1 gain on MuSiQue, a multi-hop QA benchmark. <br> &nbsp;  ✅ +9.3 average improvement across multiple long-context reasoning tasks. <br> &nbsp;  ✅ Better generalization across domains like legal, finance, and academic research. | LLM Reasoning |
| [LLM Post-Training: A Deep Dive into Reasoning Large Language Models](https://arxiv.org/pdf/2502.21321) | LLMs are trained on massive datasets. But raw pretraining isn’t enough. <br><br> Post-training is where they actually learn to reason, align with human intent, and improve factual accuracy. <br><br> This recent survey provides a systematic exploration of post-training methodologies, analyzing their role in refining LLMs beyond pretraining, addressing key challenges such as catastrophic forgetting, reward hacking, and inference-time trade-offs. <br><br> 🔑 Key Insights:  <br> &nbsp;  -> Fine-tuning helps adapt models to specific tasks but can be expensive and risks overfitting. <br> &nbsp;  -> Reinforcement learning (RL) improves adaptability but requires careful reward modeling to avoid unintended behaviors. <br> &nbsp;  -> Test-time scaling dynamically adjusts model behavior during inference, improving efficiency. <br><br> The key challenge?  <br> &nbsp;  -> Balancing accuracy, efficiency, and alignment while avoiding issues like catastrophic forgetting, reward hacking, and inference trade-offs. <br><br> And the results? <br> &nbsp;  ✅ Post-training significantly improves reasoning and factual consistency. <br> &nbsp;  ✅ RL methods like RLHF and DPO help align LLMs with user preferences. <br> &nbsp;  ✅ Fine-tuning combined with retrieval-based approaches enhances factual accuracy. | LLM Post-training |
| [How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach](https://arxiv.org/pdf/2503.01141) | LLMs can reason step by step. But are they doing it efficiently? 🧐  <br><br> Chain-of-Thought (CoT) prompting works, but it increases token usage and raises inference costs. Simply telling the model to "be concise" helps, but how much compression is too much before accuracy drops? <br><br> This is how the numbers look: <br> &nbsp;  -> Cutting response length too aggressively leads to a sharp drop in accuracy. -> Most tasks have an intrinsic token complexity - a minimum number of tokens required for correct reasoning. <br> &nbsp;  -> All compression strategies - word limits, bullet points, abbreviations - fall on a universal tradeoff curve between response length and accuracy. <br><br> This paper suggests that the LLMs need adaptive compression: <br> &nbsp;  -> Shorter reasoning for easy questions. <br> &nbsp;  -> More detailed reasoning for harder ones. <br> &nbsp;  -> Smarter compression that optimizes response length without sacrificing accuracy. <br><br> And the results? <br> &nbsp;  ✅ Up to 60% reduction in tokens while keeping accuracy intact. <br> &nbsp;  ✅ A new benchmark to measure reasoning efficiency. ✅ Insights into how LLMs can be trained to think more like humans. | Prompt compression |
| [The First Few Tokens Are All You Need: An Efficient and Effective Unsupervised Prefix Fine-Tuning Method for Reasoning Models](https://arxiv.org/pdf/2503.02875) | Fine-tuning LLMs is expensive. It requires large datasets, long training times, and massive compute. But what if the first few tokens were all you needed? <br><br> For background - this is how much fine-tuning actually improves reasoning: <br> &nbsp;  -> Full-sequence fine-tuning is wasteful - most errors happen later in the reasoning process. <br> &nbsp;  -> Models tend to start their reasoning correctly before making mistakes. <br> &nbsp;  -> If early reasoning is consistent, maybe we only need to fine-tune the first few tokens. <br><br> So, what's the alternative?
This recent paper from Tencent proposes Unsupervised Prefix Fine-Tuning (UPFT). <br> &nbsp;  -> It trains on just the first 8-32 tokens of reasoning steps, skipping full-sequence tuning. <br> &nbsp;  -> It achieves the same accuracy as full fine-tuning while cutting training cost by 75%. <br> &nbsp;  -> It reduces sampling overhead by 99%, making training dramatically more efficient. <br> &nbsp;  -> UPFT matches supervised fine-tuning, without using labeled data. <br> &nbsp;  -> Works across multiple LLM architectures, improving reasoning consistency. <br> &nbsp;  -> Proves that early reasoning steps are key to better model performance. <br><br> This is really cool. Smarter fine-tuning is the way to go! 😎  | LLM fine-tuning |
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
