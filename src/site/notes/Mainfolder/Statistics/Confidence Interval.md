---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Confidence Interval/"}
---

## 1. Fundamentals of Confidence Intervals

>
### Basic Structure and Purpose
A confidence interval takes the general form:

$$\text{statistic} \pm C \times \text{SE}$$

Where:
- [[Mainfolder/Statistics/Statistic\|statistic]] is our point estimate
- $C$ is a critical value based on desired confidence level
- SE is the [[Mainfolder/Statistics/Standard error\|standard error]] of the statistic

Purpose of confidence intervals:
- Provide a range of plausible values for an unknown [[Mainfolder/Statistics/Parameter\|parameter]]
- Account for sampling variability
- Quantify precision of our estimates

The confidence level (e.g., 95%) indicates the proportion of intervals that would contain the true parameter value if the sampling procedure was repeated many times.

## 2. Confidence Intervals for Population Means
### Formula
For a population mean ($\mu$):

$$\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$$

Where:
- $\bar{x}$ is the sample mean
- $t^*$ is the critical value from [[Mainfolder/Statistics/t-distribution\|t-distribution]]
- $s$ is the sample standard deviation
- $n$ is the sample size

### Critical Values
- For 95% confidence with normal distribution: $z^* = 1.96$
- With t-distribution: use t-value with $df = n-1$

### Conditions for Validity
1. Random sample
2. Sample size $n \geq 30$ (for normal approximation)
   - If $n < 30$, use t-distribution

## 3. Confidence Intervals for Population Proportions
### Formula
For a population proportion ($p$):

$$\hat{p} \pm z^* \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$

Where:
- $\hat{p}$ is the sample proportion
- $z^*$ is the critical value from standard normal distribution
- $n$ is the sample size

### Critical Values
Your knowledge base shows:
- 95% Confidence → $z^* = 1.96$
- 90% Confidence → $z^* = 1.645$
- 99% Confidence → $z^* = 2.576$

### Conditions for Validity
From your knowledge base:
1. Random sample
2. Success condition: $n \times \hat{p} \geq 10$
3. Failure condition: $n \times (1 - \hat{p}) \geq 10$

## 4. Confidence Intervals for Difference in Means

### Formula
For difference in population means ($\mu_1 - \mu_2$):

$$(\bar{x}_1 - \bar{x}_2) \pm t^* \times \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$$

Where:
- $\bar{x}_1$, $\bar{x}_2$ are the sample means
- $s_1$, $s_2$ are the sample standard deviations
- $n_1$, $n_2$ are the sample sizes
- $t^*$ is critical value from t-distribution

### [[Mainfolder/Statistics/degrees of freedom\|Degrees of Freedom]]
- $df = \min(n_1, n_2) - 1$

### Conditions for Validity
Your knowledge base states:
1. Random samples for both groups
2. $n_1 \geq 30$
3. $n_2 \geq 30$
4. Independent groups (values from one group don't influence values for another)

## 5. Confidence Intervals for Difference in Proportions

### Formula
For difference in population proportions ($p_1 - p_2$):

$$(\hat{p}_1 - \hat{p}_2) \pm z^* \times \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$

Where:
- $\hat{p}_1$, $\hat{p}_2$ are the sample proportions
- $n_1$, $n_2$ are the sample sizes
- $z^*$ is critical value from standard normal distribution

### Interpretation
Your knowledge base indicates that interpretation should:
- Include context
- Mention the order of comparison
- Note that positive values indicate $p_1 > p_2$, negative values indicate $p_1 < p_2$

## 6. Important Relationships and Considerations

### Trade-offs
According to your knowledge base:
- Higher confidence level → wider interval
- Larger sample size → narrower interval

### Central Limit Theorem
Your knowledge base explains the CLT is foundational for confidence intervals:
- For means: $\bar{x} \sim N(\mu, \sigma/\sqrt{n})$
- For proportions: $\hat{p} \sim N(p, \sqrt{p(1-p)/n})$

### Practical Applications
From examples in your knowledge base:
- Evaluating claims (e.g., Florida mercury levels, Chips Ahoy cookie chips)
- Comparing groups (e.g., fish caught with different nets, political attitudes)
- Medical research (e.g., survival rates of premature babies)