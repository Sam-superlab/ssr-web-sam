---
{"dg-publish":true,"permalink":"/Academic/Statistics/Confidence Interval for population mean/"}
---

# Confidence Intervals for Population Mean

## Formula and Components
- Basic formula: $\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$
- Where:
  - $\bar{x}$ = sample mean
  - $s$ = sample standard deviation
  - $n$ = sample size
  - $t^*$ = critical value from t-distribution

## Required Conditions
For a valid confidence interval:
1. Random sample from the population
2. Either:
   - Sample size $n \geq 30$, or
   - Population is normally distributed

## Normal vs. t-Distribution
- When $\sigma$ is known (rare): Use normal distribution with $\bar{x} \pm z^* \times \frac{\sigma}{\sqrt{n}}$
- When $\sigma$ is unknown (common): Use t-distribution with $\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$

## Finding Critical Values
- For 95% CI: $t_{0.975, df=n-1}$ (in R: `qt(0.975, df=n-1)`)
- For 90% CI: $t_{0.95, df=n-1}$ (in R: `qt(0.95, df=n-1)`)
- For 99% CI: $t_{0.995, df=n-1}$ (in R: `qt(0.995, df=n-1)`)

## Margin of Error
- Margin of Error (ME): $t^* \times \frac{s}{\sqrt{n}}$
- Represents the precision of your estimate

## Interpretation
"We are [confidence level]% confident that the true population mean μ is between [lower bound] and [upper bound]."

## Key Relationships
- Higher confidence level → wider interval
- Larger sample size → narrower interval

## t-Distribution Properties
- Symmetric around zero
- Bell-shaped but with heavier tails than Normal
- Approaches Normal as sample size increases
- Uses degrees of freedom (df = n-1)