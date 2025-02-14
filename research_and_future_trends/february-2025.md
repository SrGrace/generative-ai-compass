## Week 1/4
| Title | Summary | Topics |
| --- | --- | --- |
| [Memory-Efficient Fine-Tuning of Transformers via Token Selection](https://www.arxiv.org/pdf/2501.18824) | Fine-tuning LLMs is essential, but GPU memory is the bottleneck. <br><br> And this is a big deal because even the best memory-efficient methods like LoRA and QLoRA still need to cache all intermediate activations during the forward pass. <br><br> So, I looked deeper into the problem to understand: Can we fine-tune without the massive memory cost? <br><br> Here’s where TOKENTUNE comes in - a recent research from Meta AI <br><br> .. <br><br> To fine-tune a model like Llama2-7B: <br> &nbsp; -> QLoRA reduces memory usage but still needs 37% of full fine-tuning memory. <br> &nbsp; -> TOKENTUNE cuts that down further, needing just 21% of full fine-tuning memory when combined with QLoRA, saving ~79% memory overall. <br><br> How? <br> &nbsp; -> Instead of caching all tokens during backpropagation, it selects a subset of tokens for gradient computation while freezing the rest. <br> &nbsp; -> This dramatically reduces the memory footprint without hurting accuracy. <br><br> .. <br><br> So, what does this mean in practice? <br> &nbsp; 1> Fine-tuning large models becomes accessible even on smaller GPUs like the A100 or H100. <br> &nbsp; 2> Costs drop significantly for both research and deployment. <br> &nbsp; 3> It works on its own or with other methods, making it highly flexible. <br><br> But it also raises questions. <br> &nbsp; -> What happens when token selection isn’t optimal for specific tasks? <br> &nbsp;  -> Can this approach scale to models much larger than Llama2-7B? | fine-tuning |
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
