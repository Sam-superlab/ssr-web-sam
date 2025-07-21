---
{"dg-publish":true,"permalink":"/Academic/Statistics/Confidence Interval/"}
---

- [[Academic/Statistics/Confidence Interval for population mean\|Confidence Interval for population mean]]
- [[Academic/Statistics/Confidence Interval for proportions\|Confidence Interval for proportions]]
- [[Academic/Statistics/Confidence Interval for difference between groups\|Confidence Interval for difference between groups]]

# Constructing Confidence Intervals - Reference Guide

## Quick Reference Table

| Type                      | Formula                                                                                          | Critical Value                    | Conditions                                |
| ------------------------- | ------------------------------------------------------------------------------------------------ | --------------------------------- | ----------------------------------------- |
| Mean                      | $\bar{x} \pm t^* \frac{s}{\sqrt{n}}$                                                           | $t^*$ (df = $n-1$)               | $n \geq 30$ or normal                     |
| Proportion                | $\hat{p} \pm z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$                                         | $z^*$                             | $n\hat{p} \geq 10$ and $n(1-\hat{p}) \geq 10$ |
| Difference in Means       | $(\bar{x}_1-\bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$                 | $t^*$ (df = min$(n_1-1, n_2-1)$) | Independent groups                         |
| Difference in Proportions | $(\hat{p}_1-\hat{p}_2) \pm z^* \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$ | $z^*$                             | Independent groups, both satisfy conditions |

Follow these key steps when constructing confidence intervals:

## 1. Identify what you're estimating

| Parameter                | Symbol                         | Use Case               | Example                 |
| ------------------------ | ------------------------------ | ---------------------- | ----------------------- |
| Population Mean          | $\mu$                          | Quantitative variables | Height, weight, scores  |
| Population Proportion    | $p$                            | Categorical variables  | Success/failure, yes/no |
| Difference in Parameters | $\mu_1 - \mu_2$ or $p_1 - p_2$ | Group comparisons      | Treatment vs. control   |

## 2. Check appropriate conditions

### For Means
| Condition    | Requirement        | Notes                        |
| ------------ | ----------------- | ---------------------------- |
| Sample Type  | Random sample     | Essential for inference      |
| Sample Size  | $n \geq 30$       | Unless population normal     |
| Distribution | Normal if $n < 30$ | Check with Q-Q plot         |

### For Proportions
| Condition    | Requirement                | Notes                                |
| ------------ | ------------------------- | ------------------------------------ |
| Sample Type  | Random sample             | Essential for inference              |
| Success      | $n \times \hat{p} \geq 10$    | Must check BEFORE proceeding        |
| Failure      | $n \times (1-\hat{p}) \geq 10$ | Must check BEFORE proceeding        |

### For Differences
| Condition            | Requirement                                          | Notes                               |
| ------------------- | --------------------------------------------------- | ----------------------------------- |
| Independence        | Groups must be independent                           | No overlap between groups           |
| Individual Means    | Each group meets mean conditions                     | Size and normality                  |
| Individual Props    | Each group meets proportion conditions               | Success and failure conditions      |
| Degrees of Freedom  | Use df = min$(n_1-1, n_2-1)$ for difference in means | Conservative approach               |

## 3. Choose the appropriate formula

Find formula of standard error here: [[Academic/Statistics/Standard error\|standard error]]

### General Form of Confidence Interval
For any parameter $\theta$:
$$\text{Point Estimate} \pm (\text{Critical Value} \times \text{Standard Error})$$

| Parameter Type | Point Estimate | Critical Value | Standard Error |
|---------------|----------------|----------------|----------------|
| Mean | $\bar{x}$ | $t^*$ | $\frac{s}{\sqrt{n}}$ |
| Proportion | $\hat{p}$ | $z^*$ | $\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ |
| Difference in Means | $\bar{x}_1-\bar{x}_2$ | $t^*$ | $\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$ |
| Difference in Proportions | $\hat{p}_1-\hat{p}_2$ | $z^*$ | $\sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$ |

## 4. Find critical value

| Confidence Level | $z^*$ Value | Use For                |
| --------------- | ----------- | --------------------- |
| 90%             | 1.645       | Proportions          |
| 95%             | 1.96        | Proportions          |
| 99%             | 2.576       | Proportions          |
| Any             | $t^*$       | Means (check df)      |

## 5. Calculate margin of error

| Component       | Formula                         | Notes                          |
| --------------- | ------------------------------- | ------------------------------ |
| Margin of Error | Critical value × Standard Error | Use appropriate standard error |
| Standard Error  | From formula [[Academic/Statistics/Standard error\|Standard error]] | Depends on parameter type      |
|                 |                                 |                                |

## 6. Construct interval

| Component    | Formula                           | Example                             |
| ----------- | --------------------------------- | ----------------------------------- |
| Lower Bound | Point estimate - Margin of Error  | $\bar{x} - t^* \times \frac{s}{\sqrt{n}}$ |
| Upper Bound | Point estimate + Margin of Error  | $\bar{x} + t^* \times \frac{s}{\sqrt{n}}$ |

## 7. Interpret result

Template:
> "We are [confidence level]% confident that the true [parameter] lies between [lower bound] and [upper bound]."

| Component        | Example                                  | Notes                               |
| --------------- | ---------------------------------------- | ----------------------------------- |
| Confidence Level | 95%                                      | Most common choice                  |
| Parameter        | population mean                          | Be specific about what you measured |
| Bounds          | Numerical values from calculation        | Round appropriately                 |