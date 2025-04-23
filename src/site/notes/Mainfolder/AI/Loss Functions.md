---
{"dg-publish":true,"permalink":"/Mainfolder/AI/Loss Functions/"}
---


# Loss Functions

Loss functions quantify the difference between a model's predictions and the true target values. They provide the optimization objective for training neural networks and guide the learning process through [[Mainfolder/AI/Gradient Descent\|Gradient Descent]].

## Fundamental Concepts

### Purpose
- Measure prediction error
- Guide optimization process
- Define learning objective
- Enable model comparison

### Properties of Good Loss Functions
- Differentiable (for gradient-based optimization)
- Convex or locally convex
- Scale-appropriate for the task
- Computationally efficient

## Common Loss Functions

### Mean Squared Error (MSE) / L2 Loss
- Formula: $\text{MSE} = \frac{1}{n} \sum_{i=1}^n (y_i - \hat{y}_i)^2$
- Use cases:
  - Regression problems
  - Continuous output values
- Properties:
  - Heavily penalizes large errors
  - Assumes Gaussian noise
  - Always positive
  - Differentiable everywhere
- Gradient: $\frac{\partial \text{MSE}}{\partial \hat{y}_i} = -\frac{2}{n}(y_i - \hat{y}_i)$

### Cross-Entropy Loss
#### Binary Cross-Entropy
- Formula: $\text{BCE} = -(y \log(p) + (1-y)\log(1-p))$
- Use cases:
  - Binary classification
  - With [[Mainfolder/AI/Activation Functions#Sigmoid\|sigmoid]] activation
- Properties:
  - Measures information difference
  - Range: $[0, \infty)$
  - Undefined for $p = 0$ or $p = 1$

#### Categorical Cross-Entropy
- Formula: $\text{CCE} = -\sum_{k} t_k \log(y_k)$
- Use cases:
  - Multi-class classification
  - With [[Mainfolder/AI/Activation Functions#Softmax\|softmax]] activation
- Properties:
  - Generalizes binary cross-entropy
  - Handles multiple classes
  - Works with one-hot encoded targets

### Mean Absolute Error (MAE) / L1 Loss
- Formula: $\text{MAE} = \frac{1}{n} \sum_{i=1}^n |y_i - \hat{y}_i|$
- Use cases:
  - Regression with outliers
  - Robust error measurement
- Properties:
  - Less sensitive to outliers than MSE
  - Constant gradient magnitude
  - Non-differentiable at zero

### Huber Loss
- Combines MSE and MAE properties
- Formula: $$L_\delta(y, \hat{y}) = \begin{cases} 
\frac{1}{2}(y - \hat{y})^2 & \text{if } |y - \hat{y}| \leq \delta \\
\delta|y - \hat{y}| - \frac{1}{2}\delta^2 & \text{otherwise}
\end{cases}$$
- Properties:
  - Robust to outliers
  - Differentiable everywhere
  - Combines MSE and MAE benefits

## Probabilistic Interpretation

### Maximum Likelihood Connection
- MSE $\leftrightarrow$ Gaussian likelihood
- Cross-entropy $\leftrightarrow$ Bernoulli/Categorical likelihood
- See [[Mainfolder/AI/Probability and Statistics for Deep Learning\|Probability and Statistics for Deep Learning]]

### Loss Function Selection
1. Task type:
   - Regression → MSE/MAE/Huber
   - Binary classification → BCE
   - Multi-class → CCE
2. Data characteristics:
   - Outliers present → MAE/Huber
   - Gaussian noise → MSE
3. Optimization considerations:
   - Gradient behavior
   - Numerical stability

## Custom Loss Functions

### Design Principles
1. Ensure differentiability
2. Consider scale and normalization
3. Test gradient behavior
4. Balance multiple objectives

### Examples
- Weighted combinations
- Task-specific penalties
- Regularized losses (see [[Mainfolder/AI/Regularization Techniques\|Regularization Techniques]])

## Implementation Considerations

### Numerical Stability
- Use log-sum-exp trick for softmax
- Add small $\epsilon$ to avoid $\log(0)$
- Consider normalized versions

### Batch Processing
- Average loss over mini-batches
- Handle class imbalance
- Scale appropriately

### Gradients
- Check for vanishing/exploding gradients
- Monitor gradient magnitudes
- Consider gradient clipping

## Related Topics
- [[Mainfolder/AI/Neural Network Fundamentals\|Neural Network Fundamentals]] - Architecture context
- [[Mainfolder/AI/Gradient Descent\|Gradient Descent]] - Optimization process
- [[Mainfolder/AI/Backpropagation\|Backpropagation]] - Gradient computation
- [[Mainfolder/AI/Regularization Techniques\|Regularization Techniques]] - Loss modification

## References
[7] A survey and taxonomy of loss functions in machine learning
[36] MSE is Cross Entropy at heart: Maximum Likelihood Estimation Explained
[44] Loss Functions in Machine Learning Explained
[58] Loss Functions and Metrics in Deep Learning 