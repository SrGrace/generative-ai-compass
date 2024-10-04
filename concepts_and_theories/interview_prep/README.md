# Frequently asked Generative AI Interview Questions and their Answers

## Technical Foundation
1. **Describe the backpropagation algorithm.**

- Answer

  Backpropagation is an algorithm used for training neural networks. It involves computing the gradient of the loss function with respect to each weight by the chain rule, iterating backward from the output layer to the input layer. The steps are: feedforward the input to get the output, compute the loss, propagate the error back through the network by calculating the derivative of the loss with respect to each weight, and update the weights using gradient descent.

---
2. **Explain the Architecture of Transformers.**
   
- Answer:
  
  Transformers are a neural network architecture that has revolutionized natural language processing. Unlike recurrent neural networks (RNNs) and convolutional neural networks (CNNs), transformers do not process input sequentially. Instead, they rely on a self-attention mechanism to weigh the importance of different parts of the input sequence.
  
  Key Components of Transformer Architecture:
     1. Encoder-Decoder Structure: Encoder that Processes the input sequence and converts it into a meaningful representation. Decoder that Generates the output sequence based on the encoder’s output.
     2. Self-Attention Mechanism: Calculates the relevance of each word in the input sequence to every other word. Weights are assigned to words based on their importance for predicting the output. This allows the model to capture long-range dependencies in the input sequence.
     3. Multi-Head Attention: Performs multiple attention calculations simultaneously. Each attention head focuses on different aspects of the input sequence. This improves the model’s ability to capture different patterns in the data.
     4. Positional Encoding: Since transformers don’t inherently process sequential data, positional encoding is added to provide information about the order of words. This is crucial for tasks like machine translation where word order matters.
     5. Feed-Forward Neural Network: Applied to each position of the input sequence independently. Introduces non-linearity to the model.
     6. Layer Normalization: Helps stabilize training by normalizing the inputs to each layer.

   How it Works:
     1. Input Embedding: The input sequence is converted into word embeddings.
     2. Positional Encoding: Positional information is added to the word embeddings.
     3. Encoder: The input embeddings are passed through multiple encoder layers. Each layer consists of self-attention and feed-forward neural network sub-layers.
     4. Decoder: The decoder generates the output sequence one token at a time. Each decoder layer includes masked self-attention, encoder-decoder attention, and feed-forward neural network sub-layers.
     5. Output: The final output is generated through a linear layer and softmax function.

---
3. **Explain how the self-attention layer works in Transformer models.**
   
- Answer:
  
  The self-attention mechanism in Transformer models computes a weighted sum of input features for each position in the sequence, allowing the model to focus on different parts of the sequence when producing a representation for a given part. This involves three main steps: computing the Query, Key, and Value matrices, calculating attention scores using dot products of Query and Key matrices, applying a softmax function to these scores to get the attention weights, and finally computing the weighted sum of the Value matrix.

  Calculating self-attention:
  - Step 1: Calculate 3 vectors from each of the encoder's input vectors - Query(q), Key(k), Value(v) vectors
  - Step 2: Next calculate the self-attention for every word in the input sequence
    - score = $q-vector \cdot k-vector$ (dot product)
    - scores to be divided by $\sqrt{dim(v-vector)}$, in paper $dim(v-vecor)$ = 64. i.e. $score/8$
    - normalize the scores using softmax activation function

      i.e. $attention-weights(x_{1i}) = softmax(score/8)$
  - Step 3: compute the weighted sum of the value vector:
    
      $$sum_{z1} = \sum_{j=1}^{len(seq)} x_{1j}*v_j$$
    
---
4. 


## Large Language Models (LLMs)
1. **What are Large Language Models (LLM) and how do they work?**

- Answer:

  Large Language Models (LLMs) are sophisticated artificial intelligence systems designed to understand, interpret, and generate human-like text. They are built upon deep learning architectures, primarily the transformer model, and trained on massive amounts of text data. This extensive training enables LLMs to acquire a profound understanding of language patterns, grammar, semantics, and world knowledge. Top LLMs in market right now are — OpenAI's o1, GPT4, GPT4o-Mini, Meta's LLAMA3.1, 3.2, Google Gemini, Claude, Mistral, Falcon and many more.
  
  Working: LLMs primarily rely on transformer architecture, a neural network architecture that has revolutionized natural language processing.
  
  Here’s a breakdown of key components:
  
  Transformer Architecture:
    1. Encoder-Decoder Structure: This architecture processes input text (encoding) and generates output text (decoding).
    2. Self-Attention Mechanism: This allows the model to weigh the importance of different words in a sequence, capturing complex relationships between them.
    3. Multi-Head Attention: This enhances the model’s ability to focus on different aspects of the input simultaneously.
    4. Positional Encoding: Since transformers don’t inherently process sequential data, positional encoding adds information about the order of words.
    5. Pre-training: LLMs undergo a pre-training phase where they learn to predict the next word in a sequence. This unsupervised learning process helps them develop a strong language understanding foundation.
    6. Fine-tuning: For specific tasks like question answering or text summarization, LLMs are fine-tuned on smaller, task-specific datasets. This process adapts the model to excel at the desired task.


---  
2. **What are the differences between LLMs and Traditional Statistical Language Models?**

- Answer

  Large Language Models (LLMs) represent a significant leap forward from traditional statistical language models.

  Let’s explore the key differences:
  
  - Traditional Statistical Language Models:
    1. Based on statistical probabilities: These models rely on calculating the probability of a word occurring given the previous words in a sequence.
    2. Limited context understanding: They typically have a short-term memory, rely on fixed n-grams and statistical rules, making it difficult to capture long-range dependencies.
    3. Task-specific: These models are often designed for specific tasks like machine translation or speech recognition.
    4. Rule-based or probabilistic: They employ rule-based approaches or probabilistic methods for language processing.
     
  - Large Language Models (LLMs):
    1. Deep learning-based: LLMs leverage the power of neural networks, specifically transformer architecture.
    2. Massive datasets: Trained on vast amounts of text data, allowing them to learn complex language patterns.
    3. Strong contextual understanding: They can capture long-range dependencies and understand the context of a sentence or paragraph.
    4. Versatility: LLMs can be adapted to various NLP tasks with minimal fine-tuning.
    5. Generative capabilities: Beyond understanding language, LLMs can generate human-quality text, translate languages, write different kinds of creative content, and answer your questions in an informative way.

---
3.

- Answer


## Retrieval- Augmented Generation (RAG)
1. 

- Answer


---  
2. 

- Answer

---
3.

- Answer
