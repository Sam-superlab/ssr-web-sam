---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Critical Values/"}
---

# Critical Values

Critical values are the cut-off points that separate the critical region from the non-critical region in a [[Mainfolder/Statistics/hypothesis testing\|hypothesis test]] or determine the width of a [[Mainfolder/Statistics/Confidence Interval\|confidence interval]].

## Choosing Critical Values

| Distribution | When to Use | Requirements | Example Uses |
|-------------|-------------|--------------|--------------|
| z-critical ($z^*$) | Large samples | $n \geq 30$, known $\sigma$ | Proportions, large sample means |
| t-critical ($t^*$) | Small samples | $n < 30$, unknown $\sigma$ | Small sample means, differences |

## Types of Critical Values

### z-Critical Values ($z^*$)
Used with:
- [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]]
- Proportion tests and intervals

| Confidence Level | Area in Tails ($\alpha$) | $z^*$ Value |
|-----------------|-------------------------|-------------|
| 90% | 0.10 | 1.645 |
| 95% | 0.05 | 1.96 |
| 99% | 0.01 | 2.576 |

### t-Critical Values ($t^*$)
Used with:
- [[Mainfolder/Statistics/t-distribution\|t-distribution]]
- Mean-based tests and intervals

t-critical values depend on:
- Confidence level
- [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] (df = $n-1$)

## Finding Critical Values

### Process Comparison

| Step | z-Critical Values | t-Critical Values |
|------|------------------|-------------------|
| 1. Level | Choose confidence level (C) | Choose confidence level (C) |
| 2. Calculate | $\alpha = 1 - C$ | df = $n-1$ |
| 3. Find | $z^*$ for area $1-\frac{\alpha}{2}$ | $t^*$ for area $1-\frac{\alpha}{2}$ with df |
| Example | 95%: $z_{0.975} = 1.96$ | 95%, n=10: $t_{0.975,9} = 2.262$ |

## Applications in Statistical Analysis

### Confidence Intervals

| Type | Formula | When to Use |
|------|---------|-------------|
| Large Sample Mean | $\bar{x} \pm z^* \times \frac{\sigma}{\sqrt{n}}$ | $n \geq 30$, known $\sigma$ |
| Small Sample Mean | $\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$ | $n < 30$ or unknown $\sigma$ |
| Proportion | $\hat{p} \pm z^* \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ | $n\hat{p} \geq 10$, $n(1-\hat{p}) \geq 10$ |

### Hypothesis Testing Decision Rules

| Method | Decision Rule | Equivalent to |
|--------|---------------|---------------|
| Critical Value | Reject $H_0$ if $|$test statistic$| > $ critical value | Two-tailed test |
| p-value | Reject $H_0$ if p-value < $\alpha$ | Same conclusion |

## Common Values Reference Table

| Confidence Level | $\alpha$ | z-critical | t-critical (df=10) | t-critical (df=20) |
|-----------------|----------|-------------|-------------------|-------------------|
| 90% | 0.10 | 1.645 | 1.812 | 1.725 |
| 95% | 0.05 | 1.96 | 2.228 | 2.086 |
| 99% | 0.01 | 2.576 | 3.169 | 2.845 |

## Key Relationships
- Critical values ↔ Confidence level (fixed relationship)
- [[p-value\|p-value]] ↔ Test statistic (varies by sample)
- Sample size ↔ Type of critical value (z or t)

See also:
- [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]]
- [[Mainfolder/Statistics/hypothesis testing\|hypothesis testing]]
- [[Mainfolder/Statistics/Standard error\|Standard Error]]
- [[Mainfolder/Statistics/t-distribution\|t-distribution]]
- [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] 