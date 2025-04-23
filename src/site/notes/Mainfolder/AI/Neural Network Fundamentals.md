---
{"dg-publish":true,"permalink":"/Mainfolder/AI/Neural Network Fundamentals/"}
---


# Neural Network Fundamentals

Neural networks are computational models inspired by biological neural systems, composed of interconnected processing units (neurons) organized in layers. This note covers the fundamental building blocks and mathematical principles.

## Basic Components

### Neurons (Perceptrons)
- Mathematical model of a single neuron:
  - Inputs: $\mathbf{x} = [x_1, x_2, \ldots, x_n]$
  - Weights: $\mathbf{w} = [w_1, w_2, \ldots, w_n]$
  - Bias: $b$
  - Weighted sum: $z = \mathbf{w} \cdot \mathbf{x} + b$
  - Activation: $a = g(z)$ where $g$ is an [[Mainfolder/AI/Activation Functions\|activation function]]

### Weights and Biases
- Learnable parameters of the network
- Weights represent connection strengths
- Biases allow shifting the activation function
- See [[Mainfolder/AI/Linear Algebra for Deep Learning\|Linear Algebra for Deep Learning]] for matrix representation

### Layers
1. Input Layer
   - Receives raw input data
   - No computation performed
   - Size matches input dimensionality

2. Hidden Layers
   - Perform intermediate computations
   - Apply weights, biases, and activations
   - Multiple layers enable hierarchical feature learning

3. Output Layer
   - Produces final predictions
   - Architecture depends on task:
     - Regression: Linear activation
     - Binary classification: Sigmoid activation
     - Multi-class: Softmax activation

## Mathematical Representation

### Forward Propagation
For layer $l$ with $m$ neurons:
1. Matrix multiplication: $\mathbf{z}^{[l]} = \mathbf{W}^{[l]}\mathbf{a}^{[l-1]} + \mathbf{b}^{[l]}$
   - $\mathbf{W}^{[l]}$: weight matrix $(m \times n)$
   - $\mathbf{a}^{[l-1]}$: activations from previous layer $(n \times 1)$
   - $\mathbf{b}^{[l]}$: bias vector $(m \times 1)$
2. Apply activation: $\mathbf{a}^{[l]} = g(\mathbf{z}^{[l]})$

### Matrix Dimensions
- Input layer ($n_0$ neurons): $\mathbf{a}^{[0]}$ is $n_0 \times 1$
- Hidden layer $l$ ($n_l$ neurons):
  - $\mathbf{W}^{[l]}$ is $n_l \times n_{l-1}$
  - $\mathbf{b}^{[l]}$ is $n_l \times 1$
  - $\mathbf{a}^{[l]}$ is $n_l \times 1$

## Training Process Overview
1. Initialize weights and biases
2. Forward propagation to compute predictions
3. Calculate loss using [[Mainfolder/AI/Loss Functions\|Loss Functions]]
4. [[Mainfolder/AI/Backpropagation\|Backpropagation]] to compute gradients
5. Update parameters using [[Mainfolder/AI/Gradient Descent\|Gradient Descent]]
6. Repeat steps 2-5 until convergence

## Network Architectures
Different architectures are optimized for specific tasks:
- Feedforward Neural Networks (this note)
- [[Mainfolder/AI/Convolutional Neural Networks\|Convolutional Neural Networks]] for spatial data
- [[Mainfolder/AI/Recurrent Neural Networks\|Recurrent Neural Networks]] for sequential data
- [[Mainfolder/AI/Transformers\|Transformers]] for attention-based processing

## Practical Considerations
- Initialization strategies
- Learning rate selection
- [[Mainfolder/AI/Regularization Techniques\|Regularization Techniques]] to prevent overfitting
- Batch processing for computational efficiency
- Hardware optimization (GPU acceleration)

## Related Topics
- [[Mainfolder/AI/Activation Functions\|Activation Functions]] - Non-linear transformations
- [[Mainfolder/AI/Loss Functions\|Loss Functions]] - Error measurement
- [[Mainfolder/AI/Backpropagation\|Backpropagation]] - Training algorithm
- [[Mainfolder/AI/Optimization Algorithms\|Optimization Algorithms]] - Parameter updates

## References
[2] Introduction to deep learning
[10] Introduction to neural networks
[11] Neural Networks Matrix Explained
[45] Importance of Neural Network Bias 