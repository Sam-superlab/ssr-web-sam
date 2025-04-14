---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Confidence Interval for difference between groups/"}
---

# Constructing Confidence Intervals: General Guidelines

When asked to construct a confidence interval, you should generally follow these steps:

## 1. Identify what you're estimating

| Parameter Type | Symbol | Description | Example |
|---------------|--------|-------------|----------|
| Single Mean | $\mu$ | Center of one population | Average student height |
| Single Proportion | $p$ | Success rate in one population | Percentage of voters |
| Difference in Means | $\mu_1 - \mu_2$ | Difference between two population centers | Difference in test scores |
| Difference in Proportions | $p_1 - p_2$ | Difference between two population rates | Difference in success rates |

## 2. Check Validity Conditions

| Type | Conditions | Requirements |
|------|------------|--------------|
| Single Mean | Random Sample | Independent observations |
| | Sample Size/Distribution | $n \geq 30$ OR population is normal |
| Single Proportion | Random Sample | Independent observations |
| | Success-Failure | $n\hat{p} \geq 10$ AND $n(1-\hat{p}) \geq 10$ |
| Difference in Means | Independence | Between and within groups |
| | Sample Size/Distribution | Both $n \geq 30$ OR both normal |
| Difference in Proportions | Independence | Between and within groups |
| | Success-Failure | Both groups meet success-failure condition |

## 3. Formula Selection

| Scenario | Formula | Standard Error | Notes |
|----------|---------|----------------|--------|
| Single Mean | $\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$ | $\frac{s}{\sqrt{n}}$ | df = $n-1$ |
| Single Proportion | $\hat{p} \pm z^* \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ | $\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ | Use $z^*$ |
| Difference in Means | $(\bar{x}_1 - \bar{x}_2) \pm t^* \times \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$ | $\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$ | df = $\min(n_1-1, n_2-1)$ |
| Difference in Proportions | $(\hat{p}_1 - \hat{p}_2) \pm z^* \times \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$ | $\sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$ | Use $z^*$ |

## 4. Critical Value Selection

| Scenario | Distribution | Critical Value | Degrees of Freedom |
|----------|--------------|----------------|-------------------|
| Means (unknown $\sigma$) | t-distribution | $t^*$ | $n-1$ |
| Proportions | Normal | $z^*$ | N/A |
| Difference in Means | t-distribution | $t^*$ | $\min(n_1-1, n_2-1)$ |
| Difference in Proportions | Normal | $z^*$ | N/A |

Common Critical Values:
- $z^*$ (90%): 1.645
- $z^*$ (95%): 1.96
- $z^*$ (99%): 2.576
- $t^*$ values vary by df

## 5. Margin of Error Calculation
ME = critical value $\times$ standard error

## 6. Interval Construction
CI = point estimate $\pm$ margin of error

## 7. Interpretation Guidelines

| Scenario | Interpretation Template | Additional Notes |
|----------|------------------------|------------------|
| Single Parameter | "We are [C]% confident that the true [parameter] lies between [lower] and [upper]." | Specify parameter clearly |
| Difference | "We are [C]% confident that the difference ($\text{group}_1 - \text{group}_2$) lies between [lower] and [upper]." | Specify which group was subtracted |
| Contains Zero | "Since the interval contains 0, there is no significant difference between groups at the [C]% confidence level." | For difference intervals only |

Key Points:
- Always specify confidence level (C%)
- Clearly identify groups being compared
- State which group was subtracted from which
- Note practical significance of results
