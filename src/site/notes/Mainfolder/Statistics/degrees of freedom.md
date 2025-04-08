---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/degrees of freedom/"}
---

>Degrees of freedom (df) is a statistical concept that refers to the **number of independent values** that can vary in an analysis without breaking any constraints.

## Conceptual Understanding

Degrees of freedom represents the number of independent pieces of information available for estimating a parameter. It's essentially:
- The number of values that are free to vary when estimating statistical parameters
- Often calculated as sample size minus the number of parameters being estimated

## Common Applications

### In Sample Variance Calculation
- Formula: $s = \sqrt{\frac{1}{n-1} \sum (x_i - \bar{x})^2}$
- Degrees of freedom = n-1
- Why? When calculating sample variance, we've already used 1 degree of freedom to estimate the mean

### For Difference in Means
According to your personal knowledge base:
- When comparing two population means
- df = min(n₁, n₂) - 1
- This appears in confidence interval calculations for differences between two means

## Importance in Statistical Tests
Degrees of freedom determine the:
- Shape of sampling distributions
- Critical values in hypothesis tests
- Appropriate t-distribution to use
