---
{"dg-publish":true,"permalink":"/Academic/AI/Activation Functions/"}
---


# Activation Functions

Activation functions introduce non-linearity into neural networks, enabling them to learn complex patterns and relationships in data. This note covers the most common activation functions, their mathematical properties, and practical considerations.

## Purpose and Importance
- Introduce non-linearity into the network
- Enable learning of complex patterns
- Control the range of output values
- Affect gradient flow during training

## Common Activation Functions

### Sigmoid (Logistic)
- Formula: σ(z) = 1 / (1 + e^(-z))
- Range: (0, 1)
- Derivative: σ'(z) = σ(z)(1 - σ(z))
- Properties:
  - Smooth gradient
  - Output interpretable as probability
  - Suffers from vanishing gradients
  - Not zero-centered
- Use cases:
  - Binary classification (output layer)
  - Legacy networks (mostly replaced by ReLU)

### Tanh (Hyperbolic Tangent)
- Formula: tanh(z) = (e^z - e^(-z)) / (e^z + e^(-z))
- Range: (-1, 1)
- Derivative: tanh'(z) = 1 - tanh²(z)
- Properties:
  - Zero-centered
  - Stronger gradients than sigmoid
  - Still has vanishing gradient problem
- Use cases:
  - Hidden layers when zero-centered output is desired
  - RNNs and LSTMs

### ReLU (Rectified Linear Unit)
- Formula: ReLU(z) = max(0, z)
- Range: [0, ∞)
- Derivative: 1 if z > 0, 0 if z ≤ 0
- Properties:
  - Computationally efficient
  - Helps with vanishing gradient problem
  - Can suffer from "dying ReLU" problem
  - Not zero-centered
- Use cases:
  - Most common choice for hidden layers
  - Deep networks
  - [[Academic/AI/Convolutional Neural Networks\|Convolutional Neural Networks]]

### Softmax
- Formula: f(z_i) = e^(z_i) / Σ(e^(z_j))
- Range: (0, 1) with Σf(z_i) = 1
- Properties:
  - Outputs sum to 1
  - Interpretable as probabilities
  - Computationally stable with log-softmax
- Use cases:
  - Multi-class classification (output layer)
  - See [[Academic/AI/Loss Functions\|Loss Functions]] for cross-entropy loss

## Variants and Modifications

### Leaky ReLU
- Formula: f(z) = max(αz, z), where α is small (e.g., 0.01)
- Addresses dying ReLU problem
- Allows small negative gradients

### ELU (Exponential Linear Unit)
- Formula: f(z) = z if z > 0, α(e^z - 1) if z ≤ 0
- Combines ReLU benefits with negative values
- Smoother gradients

### GELU (Gaussian Error Linear Unit)
- Used in modern architectures like [[Academic/AI/Transformers\|Transformers]]
- Smooth approximation of ReLU
- Better performance in some cases

## Practical Considerations

### Selection Criteria
1. Network depth
2. Task type (classification/regression)
3. Computational resources
4. Gradient flow requirements

### Common Combinations
- Hidden layers: ReLU or variants
- Output layer:
  - Regression: Linear
  - Binary classification: Sigmoid
  - Multi-class: Softmax

### Implementation Notes
- Initialize weights appropriately for chosen activation
- Consider computational efficiency
- Monitor for activation-specific issues (e.g., dying ReLU)
- See [[Academic/AI/Neural Network Fundamentals\|Neural Network Fundamentals]] for integration

## Related Topics
- [[Academic/AI/Neural Network Fundamentals\|Neural Network Fundamentals]] - Basic architecture
- [[Academic/AI/Backpropagation\|Backpropagation]] - Gradient computation
- [[Academic/AI/Loss Functions\|Loss Functions]] - Error calculation
- [[Academic/AI/Gradient Descent\|Gradient Descent]] - Optimization process

## References
[49] Neural networks: Activation functions
[50] Activation Functions in Neural Networks Explained
[51] Activation functions in Neural Networks
[54] Introduction to Activation Functions in Neural Networks 