# Frequently asked Generative AI Interview Questions and their Answers

## Technical Foundation
1. Explain how the self-attention layer works in Transformer models.
   
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
    

2. Describe the backpropagation algorithm.
   
- Answer

  Backpropagation is an algorithm used for training neural networks. It involves computing the gradient of the loss function with respect to each weight by the chain rule, iterating backward from the output layer to the input layer. The steps are: feedforward the input to get the output, compute the loss, propagate the error back through the network by calculating the derivative of the loss with respect to each weight, and update the weights using gradient descent.

3.

## Large Language Models
1. 
- Answer


  
2. 
- Answer

3.


## Retrieval- Augmented Generation (RAG)
1. 
- Answer


  
2. 
- Answer

3.
