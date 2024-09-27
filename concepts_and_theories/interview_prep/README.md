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


## Large Language Models
1. 
- Answer


---  
2. 
- Answer

---
3.


## Retrieval- Augmented Generation (RAG)
1. 
- Answer


---  
2. 
- Answer

---
3.
