## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Chain-of-Thought Matters: Improving Long-Context Language Models with Reasoning Path Supervision](https://arxiv.org/pdf/2502.20790) | LLMs struggle with long-context reasoning. 🫠 <br><br> They can read thousands of tokens, but pulling the right information and reasoning through it? That’s where things fall apart. <br><br> So, I looked at why this happens. <br> &nbsp;  -> LLMs often retrieve the wrong information from long documents. <br> &nbsp;  -> Chain-of-Thought (CoT) helps, but not always - sometimes it adds unnecessary steps. <br> &nbsp;  -> Even when CoT works, models don’t learn how to reason better over time. <br><br> What’s the fix?  <br><br> This recent paper proposes LONGREPS - a process-supervised approach that teaches LLMs how to reason over long contexts. It -  <br> &nbsp;  -> Bootstraps reasoning paths by letting the model generate multiple solutions. <br> &nbsp;  -> Filters out low-quality reasoning using a new quality assessment method. <br> &nbsp;  -> Fine-tunes models on only high-quality reasoning paths to improve long-context understanding. <br><br> And the results? <br> &nbsp;  ✅ +13.6 F1 gain on MuSiQue, a multi-hop QA benchmark. <br> &nbsp;  ✅ +9.3 average improvement across multiple long-context reasoning tasks. <br> &nbsp;  ✅ Better generalization across domains like legal, finance, and academic research. | LLM Reasoning |
| [LLM Post-Training: A Deep Dive into Reasoning Large Language Models](https://arxiv.org/pdf/2502.21321) | LLMs are trained on massive datasets. But raw pretraining isn’t enough. <br><br> Post-training is where they actually learn to reason, align with human intent, and improve factual accuracy. <br><br> This recent survey provides a systematic exploration of post-training methodologies, analyzing their role in refining LLMs beyond pretraining, addressing key challenges such as catastrophic forgetting, reward hacking, and inference-time trade-offs. <br><br> 🔑 Key Insights:  <br> &nbsp;  -> Fine-tuning helps adapt models to specific tasks but can be expensive and risks overfitting. <br> &nbsp;  -> Reinforcement learning (RL) improves adaptability but requires careful reward modeling to avoid unintended behaviors. <br> &nbsp;  -> Test-time scaling dynamically adjusts model behavior during inference, improving efficiency. <br><br> The key challenge?  <br> &nbsp;  -> Balancing accuracy, efficiency, and alignment while avoiding issues like catastrophic forgetting, reward hacking, and inference trade-offs. <br><br> And the results? <br> &nbsp;  ✅ Post-training significantly improves reasoning and factual consistency. <br> &nbsp;  ✅ RL methods like RLHF and DPO help align LLMs with user preferences. <br> &nbsp;  ✅ Fine-tuning combined with retrieval-based approaches enhances factual accuracy. | LLM Post-training |
| []() |  |  |
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
