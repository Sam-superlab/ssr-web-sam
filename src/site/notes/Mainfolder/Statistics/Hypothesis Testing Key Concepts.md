---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Key Concepts/"}
---


## Key Concepts in Hypothesis Testing

### Null Distribution
* The distribution of sample statistics that would occur if the null hypothesis ($H_0$) were true
* Simulates the world under the "no effect" assumption
* For means and proportions, under certain conditions (like random sampling and sufficient sample size via the [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]]), the null distribution often resembles a [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]]
* Its center is the hypothesized value from $H_0$ (e.g., $p_0$, $\mu_0$)
* The spread depends on the [[Mainfolder/Statistics/Standard error\|Standard error]] calculated under $H_0$ assumptions

### Test Statistic
* A standardized value that simplifies comparing the sample statistic to the null distribution
* Measures the difference between the sample statistic and the null hypothesis value in terms of standard errors
* General Formula: $\frac{\text{Sample Statistic} - \text{Null Hypothesis Value}}{\text{Standard Error}}$
* Purpose: Converts the sample result into a score on a known standard distribution ([[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] or [[Mainfolder/Statistics/t-distribution\|t-distribution]])
* Makes calculating the p-value straightforward using functions like `pnorm()` or `pt()`

### P-value
* The probability of obtaining an observed statistic (or test statistic) equal to or more extreme than the one actually observed, assuming the null hypothesis ($H_0$) is true
* Interpretation:
  * Small p-value: Observed data is unlikely if $H_0$ were true, providing strong evidence against $H_0$
  * Large p-value: Observed data is plausible under $H_0$, providing weak or no evidence against $H_0$
* Calculation depends on $H_a$:
  * Right-tailed ($H_a: >$): Area to the right of the test statistic
  * Left-tailed ($H_a: <$): Area to the left of the test statistic
  * Two-tailed ($H_a: \neq$): Area in both tails beyond the absolute value of the test statistic

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction to hypothesis testing
* [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Application of these concepts to proportion tests
* [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Application of these concepts to mean tests
* [[Mainfolder/Statistics/Critical Values\|Critical Values]] - Important values for making decisions in hypothesis testing
* [[Mainfolder/Statistics/Standard error\|Standard error]] - Understanding the denominator in test statistics
* [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] - Important concept for t-distribution tests
* [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] - Foundation for understanding null distributions
* [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] - Common distribution for test statistics 