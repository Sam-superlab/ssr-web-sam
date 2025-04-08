---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/t-distribution/"}
---

When working with small samples or when the **population standard deviation is unknown, we use the t-distribution.**
### Key Properties
- Symmetric around zero
- Bell-shaped like the Normal distribution
- Characterized by [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] (df = n - 1)
- Has heavier tails than the Normal distribution
- Approaches the Normal distribution as sample size increases (n → $\infty$)

### Comparing Normal and t-Distributions

From your knowledge base:
- t-distribution requires wider intervals due to heavier tails
- As sample size increases, t-distribution converges to Normal

## Confidence Intervals Using These Distributions

### Normal Distribution (Large Samples)

For 95% confidence intervals when σ is known or n ≥ 30:
- x̄ ± 1.96 × (σ/√n)

### t-Distribution (Small Samples)

For small samples or unknown σ:
- x̄ ± t₀.₉₇₅,ₙ₋₁ × (s/√n)
- Where t₀.₉₇₅,ₙ₋₁ is the 97.5th percentile of the t-distribution with n-1 degrees of freedom

### Trade-offs in Confidence Intervals

From your knowledge base:
- Higher confidence level → Wider interval
- Lower confidence level → Narrower interval
- Larger sample size → Narrower interval

## Conditions for Valid Application

For the Normal approximation to be valid:
1. Random sample from the population
2. Sample size n ≥ 30 (otherwise, use t-distribution)

For t-distribution to be valid:
1. Random sample
2. The population should be approximately normally distributed if n is small
