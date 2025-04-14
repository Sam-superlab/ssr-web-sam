---
dg-publish: true
---

## Hypothesis Testing for Means

### Single Population Mean ($\mu$)
| Component | Description |
|-----------|-------------|
| Parameter | $\mu$ (population mean) |
| Statistic | $\bar{x}$ (sample mean) |
| Hypotheses | $H_0: \mu = \mu_0$ <br> $H_a: \mu < \mu_0$ or $H_a: \mu > \mu_0$ or $H_a: \mu \neq \mu_0$ |
| Conditions | 1. [[Mainfolder/Statistics/Simple Random Sample (SRS)\|Simple Random Sample (SRS)]] <br> 2. [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] population OR $n \geq 30$ (by [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]]) |
| Test Statistic | Known $\sigma$: $Z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}$ <br> Unknown $\sigma$: $T = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$ |
| Distribution | Known $\sigma$: [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] $N(0,1)$ <br> Unknown $\sigma$: [[Mainfolder/Statistics/t-distribution\|t-distribution]] with $df = n-1$ |

### Difference of Two Population Means ($\mu_1 - \mu_2$)
| Component | Description |
|-----------|-------------|
| Parameter | $\mu_1 - \mu_2$ (difference in population means) |
| Statistic | $\bar{x}_1 - \bar{x}_2$ (difference in sample means) |
| Hypotheses | $H_0: \mu_1 - \mu_2 = 0$ <br> $H_a: \mu_1 - \mu_2 < 0$ or $H_a: \mu_1 - \mu_2 > 0$ or $H_a: \mu_1 - \mu_2 \neq 0$ |
| Conditions | 1. [[Mainfolder/Statistics/Simple Random Sample (SRS)\|Simple Random Sample (SRS)]] from two independent groups <br> 2. [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] populations OR both $n_1 \geq 30$ and $n_2 \geq 30$ |
| Test Statistic | Known $\sigma$'s: $Z = \frac{\bar{x}_1 - \bar{x}_2}{\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}}$ <br> Unknown $\sigma$'s: $T = \frac{\bar{x}_1 - \bar{x}_2}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}$ |
| Distribution | Known $\sigma$'s: [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] $N(0,1)$ <br> Unknown $\sigma$'s: [[Mainfolder/Statistics/t-distribution\|t-distribution]] with $df = \min(n_1-1, n_2-1)$ |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction to hypothesis testing
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Understanding null distribution, test statistics, and p-values
* [[Mainfolder/Statistics/Confidence Interval for population mean\|Confidence Interval for population mean]] - Alternative approach to inference about means
* [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Theoretical foundation for normal approximation
* [[Mainfolder/Statistics/Standard error\|Standard error]] - Understanding the denominator in test statistics
* [[Mainfolder/Statistics/t-distribution\|t-distribution]] - Distribution used when population standard deviation is unknown
* [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] - Important concept for t-distribution tests
* [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] - Distribution used when population standard deviation is known 