---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing for Proportions/"}
---


## Hypothesis Testing for Proportions

### Single Population Proportion ($p$)
| Component | Description |
|-----------|-------------|
| Parameter | $p$ (population proportion) |
| Statistic | $\hat{p}$ (sample proportion) |
| Hypotheses | $H_0: p = p_0$ <br> $H_a: p < p_0$ or $H_a: p > p_0$ or $H_a: p \neq p_0$ |
| Conditions | 1. [[Mainfolder/Statistics/Simple Random Sample (SRS)\|Simple Random Sample (SRS)]] <br> 2. Large Enough Sample: $n \times p_0 \geq 10$ and $n \times (1 - p_0) \geq 10$ |
| Test Statistic | $Z = \frac{\hat{p} - p_0}{\sqrt{p_0(1-p_0)/n}}$ |
| Distribution | [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] $N(0,1)$ under $H_0$ |

### Difference of Two Population Proportions ($p_1 - p_2$)
| Component | Description |
|-----------|-------------|
| Parameter | $p_1 - p_2$ (difference in population proportions) |
| Statistic | $\hat{p}_1 - \hat{p}_2$ (difference in sample proportions) |
| Hypotheses | $H_0: p_1 - p_2 = 0$ <br> $H_a: p_1 - p_2 < 0$ or $H_a: p_1 - p_2 > 0$ or $H_a: p_1 - p_2 \neq 0$ |
| Pooled Proportion | $\hat{p}_{\text{pool}} = \frac{x_1 + x_2}{n_1 + n_2} = \frac{n_1\hat{p}_1 + n_2\hat{p}_2}{n_1 + n_2}$ |
| Conditions | 1. [[Mainfolder/Statistics/Simple Random Sample (SRS)\|Simple Random Sample (SRS)]] from two independent groups <br> 2. Large Enough Samples: $n_1\hat{p}_{\text{pool}} \geq 10$, $n_1(1-\hat{p}_{\text{pool}}) \geq 10$, $n_2\hat{p}_{\text{pool}} \geq 10$, $n_2(1-\hat{p}_{\text{pool}}) \geq 10$ |
| Test Statistic | $Z = \frac{\hat{p}_1 - \hat{p}_2}{\sqrt{\hat{p}_{\text{pool}}(1-\hat{p}_{\text{pool}})(\frac{1}{n_1} + \frac{1}{n_2})}}$ |
| Distribution | [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] $N(0,1)$ under $H_0$ |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction to hypothesis testing
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Understanding null distribution, test statistics, and p-values
* [[Mainfolder/Statistics/Confidence Interval for proportions\|Confidence Interval for proportions]] - Alternative approach to inference about proportions
* [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Theoretical foundation for normal approximation
* [[Mainfolder/Statistics/Standard error\|Standard error]] - Understanding the denominator in test statistics
* [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] - Distribution used for proportion tests 