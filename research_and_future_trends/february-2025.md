## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Memory-Efficient Fine-Tuning of Transformers via Token Selection](https://www.arxiv.org/pdf/2501.18824) | Fine-tuning LLMs is essential, but GPU memory is the bottleneck. <br><br> And this is a big deal because even the best memory-efficient methods like LoRA and QLoRA still need to cache all intermediate activations during the forward pass. <br><br> So, I looked deeper into the problem to understand: Can we fine-tune without the massive memory cost? <br><br> Here’s where TOKENTUNE comes in - a recent research from Meta AI <br><br> .. <br><br> To fine-tune a model like Llama2-7B: <br><br> &nbsp; -> QLoRA reduces memory usage but still needs 37% of full fine-tuning memory. <br><br> &nbsp; -> TOKENTUNE cuts that down further, needing just 21% of full fine-tuning memory when combined with QLoRA, saving ~79% memory overall. <br><br> How? <br><br> &nbsp; -> Instead of caching all tokens during backpropagation, it selects a subset of tokens for gradient computation while freezing the rest. <br><br> &nbsp; -> This dramatically reduces the memory footprint without hurting accuracy. <br><br> .. <br><br> So, what does this mean in practice? <br><br> &nbsp; 1> Fine-tuning large models becomes accessible even on smaller GPUs like the A100 or H100. <br><br> &nbsp; 2> Costs drop significantly for both research and deployment. <br><br> &nbsp; 3> It works on its own or with other methods, making it highly flexible. <br><br> But it also raises questions. <br><br> &nbsp; -> What happens when token selection isn’t optimal for specific tasks? <br><br> &nbsp;  -> Can this approach scale to models much larger than Llama2-7B? | fine-tuning |
| [SETS: Leveraging Self-Verification and Self-Correction for Improved Test-Time Scaling](https://arxiv.org/pdf/2501.19306) | Improving LLM performance during inference is always tricky. <br><br> And this is a big deal because traditional methods like repeated sampling or task-specific reward models quickly hit diminishing returns as compute scales. <br><br> So, I looked into Google's SETS (Self-Enhanced Test-Time Scaling) to see how it tackles this challenge differently. <br><br> .. <br><br> To improve outputs, most methods rely on sampling multiple responses and using majority votes. But here’s the catch: <br><br> &nbsp; -> As the number of samples increases, performance gains plateau. <br><br> &nbsp; -> Adding a task-specific reward model to verify solutions drives up costs and reduces scalability. <br><br> SETS takes a different approach. <br><br> .. <br><br> Instead of relying on just sampling: <br><br> &nbsp; -> It introduces Self-Verification to check if an answer meets constraints. <br><br> &nbsp; -> Then uses Self-Correction to refine incorrect responses. <br><br> &nbsp; -> This iterative process improves responses while keeping costs under control.<br><br> And the results? <br><br> &nbsp; -> On tasks like trip and meeting planning (NATURAL PLAN benchmark), SETS improved accuracy by up to 8.7% over repeated sampling. <br><br> &nbsp;  -> Confidence scores also got better, with up to 9% higher AUACC and reduced calibration errors, ensuring more reliable outputs. <br><br> .. <br><br> But the real kicker is efficiency: <br><br> SETS doesn’t need external reward models or extra fine-tuning. It works with existing LLM capabilities, making it scalable across tasks. <br><br> However, the effectiveness of SETS depends heavily on the underlying model's self-verification and correction abilities. Stronger these are, the better SETS performs. | LLM Reasoning |
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
