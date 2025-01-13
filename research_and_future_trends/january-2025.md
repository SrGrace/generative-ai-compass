## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [CODEELO: Benchmarking Competition-level Code Generation of LLMs with Human-comparable Elo Ratings](https://arxiv.org/pdf/2501.01257) | For years, we've wondered, how do coding LLMs really stack up against human developers? <br><br> Most benchmarks have fallen short, offering unrealistic test cases or missing the nuances of real-world programming challenges. <br><br> CODEELO: a new benchmark - addresses this by integrating directly with CodeForces, the global hub for competitive programming. 🌐 <br><br> 🔑 Key Insights: <br> &nbsp; 🔹 Real Problems, Real Stakes: It uses CodeForces problems, test cases, and conditions - just like human participants face. <br> &nbsp; 🔹 Elo Ratings for LLMs: CODEELO assigns ratings comparable to human players, offering unprecedented insight into LLM capabilities. <br> &nbsp; 🥇 Only two models, OpenAI’s o1-mini (1578) and QwQ-32B-Preview (1261), scored above 1200 Elo. Most others? Stuck in the bottom 20% of human participants. <br> &nbsp; 🧠 Strengths and Weaknesses: Top models excel in math but falter with dynamic programming and complex data structures. | Coding Benchmark |
| [Metadata Conditioning Accelerates Language Model Pre-training](https://arxiv.org/pdf/2501.01956) | This new research introduces MeCo (Metadata Conditioning then Cooldown), a method that brings simplicity, efficiency, and control to language model pre-training.  <br><br> 🔑 Here’s why this approach is so compelling: <br> &nbsp; ✅ Efficient Pre-training: MeCo uses metadata like URLs (e.g., en.wikipedia.org) during training to provide contextual cues, enabling the model to group and learn from documents more effectively. This reduces training data requirements by 33% - a 1.6B model achieves standard pre-training performance with fewer resources. <br> &nbsp; ✅ Steerable AI: By conditioning inference on metadata, even fabricated ones (e.g., factquizmaster.com), we can influence model behaviour. This reduces toxic outputs and boosts task-specific performance. <br> &nbsp; ✅ Universal Applicability: Compatible across model scales (600M to 8B parameters) and training datase | LLM Pre-Training |
| [AdaSkip: Adaptive Sublayer Skipping for Accelerating Long-Context LLM Inference](https://arxiv.org/pdf/2501.02336) | As LLMs tackle longer and longer texts (some now handling 1M+ tokens!), making them run efficiently becomes crucial. <br><br> This recent research proposes AdaSkip - it offers a practical solution without the complex training or fine-tuning needed by other methods - a smart way to accelerate LLMs when dealing with long text! <br><br> 🔑 Key highlights: <br> &nbsp; 🔹 Unlike previous approaches that skip entire layers, AdaSkip intelligently identifies and skips less important sub-components, maintaining model quality while boosting speed <br> &nbsp; 🔹 Works during both "prefilling" (initial processing) and "decoding" (generation) phases <br> &nbsp; 🔹 Adapts automatically to different models and contexts - no one-size-fits-all approach!  <br> &nbsp; 🔹 Achieved impressive results across multiple models (LLaMA, InternLM, Vicuna) and tasks | LLM Inference |
| [RAG-Check: Evaluating Multimodal Retrieval Augmented Generation Performance](https://arxiv.org/pdf/2501.03995) | Combining text, images, and more, multimodal RAG unlocks incredible potential - but it also opens the door to new challenges. Chief among them? Hallucination. <br><br> 🚨 Hallucinations in multimodal RAG systems stem from three layers:  <br> &nbsp;  1️⃣ Selection-hallucination: When irrelevant data (e.g., images, documents) are retrieved. <br> &nbsp;  2️⃣ Context-generation-hallucination: When vision-LMs generate inaccurate textual descriptions of visual data. <br> &nbsp;  3️⃣ Response-generation-hallucination: When LLMs produce irrelevant or incorrect responses despite good context. <br><br> 🧪 RAG-Check: This new Framework tackles these issues head-on by introducing two novel metrics to evaluate reliability: <br> &nbsp;  🔍 Relevance Score (RS): How relevant is the retrieved data? <br> &nbsp;  ✔️ Correctness Score (CS): How accurate are the generated responses? <br><br> 🎯 Key results? <br> &nbsp;  🔹 Both models achieve 88% accuracy on test data. <br> &nbsp;  🔹 The CS metric aligns with human evaluations 91% of the time, and RS outperforms traditional measures by over 20%! <br><br> 🔖 As multimodal RAG becomes mainstream, the conversation around hallucination detection and reliability metrics will only grow louder. Papers like this could define the standards for what comes next. | Multimodal RAG Evaluation |
| [Understanding Before Reasoning: Enhancing Chain-of-Thought with Iterative Summarization Pre-Prompting](https://arxiv.org/pdf/2501.04341) | This recent paper introduces Iterative Summarization Pre-Prompting (ISP2), a novel pre-prompting technique designed to enhance the reasoning capabilities of LLMs by refining the input context before reasoning starts. <br><br> Traditional Chain-of-Thought (CoT) prompting focuses on breaking down reasoning into steps but often struggles when essential information is missing or implicit.  <br><br> 💡 ISP2 tackles this by:  <br> &nbsp; 1️⃣ Extracting entities and key descriptions to form "information pairs." <br> &nbsp;  2️⃣ Iteratively merging and refining these pairs using a reliability rating system. <br> &nbsp;  3️⃣ Feeding the refined context back to the LLM for better reasoning. <br><br> 📈 The Results: <br> &nbsp;  🔹 A 7.1% improvement in reasoning tasks when combined with CoT. <br> &nbsp;  🔹 Exceptional plug-and-play compatibility across models  <br> &nbsp;  🔹 Significant advancements in commonsense and reasoning benchmarks. <br><br> 🤖 By focusing on understanding the problem space through iterative summarization, ISP2 enables LLMs to generate more accurate, contextually rich answers.  | Pre-Prompting |
| []() |  |  |
| []() |  |  |

## Week 2/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |
| []() |  |  |


## Week 3/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |
| []() |  |  |


## Week 4/4
| Title | Summary | Topics |
| --- | --- | --- |
| []() |  |  |
| []() |  |  |
| []() |  |  |
