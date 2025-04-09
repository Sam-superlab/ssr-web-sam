---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/t-distribution/"}
---

## t-Distribution

When working with small samples or when the **population standard deviation is unknown, we use the t-distribution.**

### Key Properties
- Symmetric around zero
- Bell-shaped like the [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]]
- Characterized by [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] (df = $n - 1$)
- Has heavier tails than the Normal distribution
- Approaches the Normal distribution as sample size increases ($n \to \infty$)

### Comparing Normal and t-Distributions

| Aspect              | t-Distribution         | Normal Distribution       |
| ------------------- | ---------------------- | ------------------------- |
| Tail Weight         | Heavier tails          | Standard tails            |
| Sample Size         | Best for small samples | Best for large samples    |
| Parameters          | Degrees of freedom     | Mean and variance         |
| [[Mainfolder/Statistics/Critical Values\|Critical Values]] | Varies with df         | Fixed values (e.g., 1.96) |
|                     |                        |                           |

## Confidence Intervals

### Using Normal Distribution ($n \geq 30$)
For 95% confidence intervals when $\sigma$ is known or $n \geq 30$:

$$\bar{x} \pm 1.96 \times \frac{\sigma}{\sqrt{n}}$$

### Using t-Distribution (Small Samples)
For small samples or unknown $\sigma$:

$$\bar{x} \pm t_{\alpha/2, n-1} \times \frac{s}{\sqrt{n}}$$

where $t_{\alpha/2, n-1}$ is the critical value from t-distribution with $n-1$ degrees of freedom

### Effect of Parameters on Intervals

The width of confidence intervals depends on:
- **Confidence Level**: Higher → Wider interval
- **Sample Size**: Larger → Narrower interval
- **Variability**: More variable → Wider interval

## Conditions for Valid Application

### For Normal Distribution
1. Random sample from the population
2. Sample size $n \geq 30$

### For t-Distribution
1. Random sample from the population
2. For small $n$: Population should be approximately normal
3. Independent observations

### When to Use Each
- Use t-distribution when:
  * Sample size is small ($n < 30$)
  * Population standard deviation ($\sigma$) is unknown
  * Working with differences in means
- Use Normal distribution when:
  * Sample size is large ($n \geq 30$)
  * Population standard deviation is known
  * Working with proportions

See also:
- [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]]
- [[Mainfolder/Statistics/Standard error\|Standard Error]]
- [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]]
