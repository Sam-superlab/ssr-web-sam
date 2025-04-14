---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing for Means/"}
---


## Hypothesis Testing for Means

### Overview

| Aspect | Description |
|--------|-------------|
| Purpose | Test claims about population means |
| Common Tests | - One-sample t-test <br> - Two-sample t-test <br> - Paired t-test |
| Assumptions | - Random sampling <br> - Normal distribution or large sample size <br> - Equal variances (for two-sample tests) |

### One-Sample t-test

| Component | Description |
|-----------|-------------|
| Purpose | Test if population mean equals a specific value |
| Hypotheses | $H_0: \mu = \mu_0$ <br> $H_a: \mu \neq \mu_0$ (or $>$, $<$) |
| Test Statistic | $t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$ |
| Degrees of Freedom | $n-1$ |

### Two-Sample t-test

| Component | Description |
|-----------|-------------|
| Purpose | Compare means of two independent populations |
| Hypotheses | $H_0: \mu_1 = \mu_2$ <br> $H_a: \mu_1 \neq \mu_2$ (or $>$, $<$) |
| Test Statistic | $t = \frac{(\bar{x}_1 - \bar{x}_2) - (\mu_1 - \mu_2)}{s_p\sqrt{\frac{1}{n_1} + \frac{1}{n_2}}}$ |
| Degrees of Freedom | $n_1 + n_2 - 2$ |

### Paired t-test

| Component | Description |
|-----------|-------------|
| Purpose | Compare means of paired/matched observations |
| Hypotheses | $H_0: \mu_d = 0$ <br> $H_a: \mu_d \neq 0$ (or $>$, $<$) |
| Test Statistic | $t = \frac{\bar{d} - 0}{s_d/\sqrt{n}}$ |
| Degrees of Freedom | $n-1$ |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction to hypothesis testing
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Core concepts in hypothesis testing
* [[Mainfolder/Statistics/t-distribution\|t-distribution]] - Distribution used for mean tests
* [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] - Important concept for t-tests
* [[Mainfolder/Statistics/Standard error\|Standard error]] - Understanding the denominator in test statistics
* [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] - Foundation for understanding test statistics
* [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] - Related distribution for large samples 