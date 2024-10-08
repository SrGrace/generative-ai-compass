# Best Gen AI Papers of the month - weekly updates (October 2024)

## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Were RNNs All We Needed?](https://arxiv.org/pdf/2410.01201) | 🔍 Key Takeaways: <br> &nbsp; 🔹 Scalability Limitations: While Transformers perform well, their quadratic complexity makes them expensive for long sequences. <br> &nbsp; 🔹 Revisiting RNNs: The authors propose minimal versions of LSTMs and GRUs—minLSTM and minGRU—that remove hidden states from input, forget and update gates, making them: <br> &nbsp; &nbsp; 💨 175x-235x faster to train (for a sequence length of 512). <br> &nbsp; &nbsp; 🔢 Use significantly fewer parameters. <br> &nbsp; - This is possible because now these architectures no longer require backpropagate through time (BPTT). <br> &nbsp; 🔹 Performance Parity: Despite their simplicity, minLSTMs and minGRUs achieve performance comparable to cutting-edge models like Mamba, showing that RNNs still have a lot to offer! | RNN |
| [LLMs Know More Than They Show!](https://arxiv.org/pdf/2410.02707) | 🔑 Key Insights: <br> &nbsp; 🔹 Truthfulness is Token-Based: The research reveals that the information about the accuracy of LLM outputs is concentrated in specific tokens within the text. By focusing on these tokens, error detection methods can be significantly improved. <br> &nbsp; 🔹 Predicting Errors: Beyond detecting inaccuracies, the study found that LLMs’ internal representations can predict the types of errors they might produce—this is interesting, it could lead to tailored error mitigation strategies. <br> &nbsp; 🔹 The Model-Behaviour Mismatch: One of the most intriguing findings is the discrepancy between the model’s internal knowledge and its external output. As the authors put it: "LLMs may encode the correct answer, yet consistently generate an incorrect one." This mismatch points to the untapped potential within LLMs, offering an opportunity to develop strategies that leverage this internal knowledge and reduce hallucinations. <br><br>💡 Key Takeaways: <br> &nbsp; 🔸 By diving deeper into how LLMs process truthfulness internally, we can better understand their limitations and unlock new approaches to enhance reliability.  <br> &nbsp; 🔸 As AI continues to integrate into critical applications, these findings can play a pivotal role in shaping safer, more accurate systems. | LLMs |
| [SELECTIVE ATTENTION IMPROVES TRANSFORMER](https://arxiv.org/pdf/2410.02703) | 🪆 𝗛𝗼𝘄 𝗶𝘁 𝘄𝗼𝗿𝗸𝘀: <br> &nbsp; 1️⃣ Soft-Mask Creation: For each token, a soft-mask matrix is generated. This matrix indicates how much attention each token should give to others, with irrelevant tokens receiving less attention. <br> &nbsp; 2️⃣ Apply Constraints: The soft-mask matrix is constrained so that tokens can't mask themselves, and only future tokens are masked. <br> &nbsp; 3️⃣ Accumulate Masking: The mask is accumulated over tokens, reducing the attention paid to less relevant tokens over time. <br> &nbsp; 4️⃣ Adjust Attention Logits: The accumulated mask is subtracted from the attention logits before applying softmax, ensuring that less important tokens have reduced influence. <br> &nbsp; 5️⃣ Context Pruning: Irrelevant tokens that have been heavily masked are pruned from the attention buffer, reducing memory and computation during inference.<br><br>🔑 𝗞𝗲𝘆 𝗕𝗲𝗻𝗲𝗳𝗶𝘁𝘀: <br> &nbsp; 🔹 Improved Model Performance: Transformers equipped with selective attention outperform those with 2x the parameters and heads! <br> &nbsp; 🔹 Memory Efficiency: Reduces memory requirements by up to 47x in large context sizes, making it a game-changer for resource-constrained applications. <br> &nbsp; 🔹 Scalable Across Model Sizes: Works consistently across different model sizes and improves accuracy on challenging benchmarks like HellaSwag. | Transformers |
| []() |  |  |
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
