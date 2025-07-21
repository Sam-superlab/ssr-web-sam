---
{"dg-publish":true,"permalink":"/Academic/Statistics/Hypothesis Testing Procedure/"}
---


# Hypothesis Testing Procedure

## Overview

Hypothesis testing is a systematic process for making statistical inferences about population parameters based on sample data. This guide outlines the step-by-step procedure for conducting hypothesis tests.

## Step-by-Step Procedure

### 1. State the Hypotheses

#### Null Hypothesis ($H_0$)
- Represents the status quo or no effect
- Always includes an equality sign ($=$, $\leq$, or $\geq$)
- Example: $H_0: \mu = 100$ (population mean equals 100)

#### Alternative Hypothesis ($H_a$)
- Represents what we aim to find evidence for
- Never includes an equality sign
- Can be one-tailed ($>$ or $<$) or two-tailed ($\neq$)
- Example: $H_a: \mu > 100$ (population mean is greater than 100)

### 2. Choose Significance Level ($\alpha$)

- Common values: 0.05 (5%) or 0.01 (1%)
- Represents the probability of Type I error
- Determines the critical value(s)
- Example: $\alpha = 0.05$ means we're willing to accept a 5% chance of rejecting $H_0$ when it's true

### 3. Select Appropriate Test

Consider:
- Type of data (quantitative/categorical)
- Number of samples
- Sample size
- Distribution assumptions
- Parameter of interest (mean, proportion, variance, etc.)

Common tests:
- One-sample $t$-test
- Two-sample $t$-test
- ANOVA
- Chi-square test
- $z$-test for proportions

### 4. Calculate Test Statistic

- Formula depends on the chosen test
- Standardizes the observed difference
- Example for one-sample $t$-test:
  $t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$

### 5. Determine Critical Value(s)

- Based on:
  - Significance level ($\alpha$)
  - Degrees of freedom
  - Test direction (one/two-tailed)
- Example: For $\alpha = 0.05$ and two-tailed $t$-test with $df = 24$:
  Critical values = $\pm 2.064$

### 6. Make Decision

#### Using Critical Value Method:
- Compare test statistic to critical value(s)
- Reject $H_0$ if test statistic falls in rejection region
- Example: If $|t| > 2.064$, reject $H_0$

#### Using P-value Method:
- Calculate p-value (probability of more extreme results)
- Reject $H_0$ if p-value < $\alpha$
- Example: If p-value = 0.03 < 0.05, reject $H_0$

### 7. State Conclusion

- Clear statement about the decision
- Include context and practical significance
- Example: "We reject the null hypothesis at $\alpha = 0.05$, suggesting that the new teaching method significantly improves test scores."

## Common Pitfalls to Avoid

1. **Multiple Testing**
   - Performing multiple tests increases Type I error
   - Use appropriate corrections (Bonferroni, etc.)

2. **Data Dredging**
   - Testing multiple hypotheses without pre-specification
   - Increases false positive rate

3. **Misinterpreting P-values**
   - P-value is not the probability that $H_0$ is true
   - Small p-value doesn't guarantee practical significance

4. **Ignoring Assumptions**
   - Each test has specific assumptions
   - Violating assumptions can invalidate results

## Example: One-Sample t-test

### Scenario
Testing if a new teaching method improves test scores (known population mean = 75)

### Steps
1. **Hypotheses**
   - $H_0: \mu = 75$
   - $H_a: \mu > 75$

2. **Significance Level**
   - $\alpha = 0.05$

3. **Test Selection**
   - One-sample $t$-test (comparing mean to known value)

4. **Test Statistic**
   - Sample mean = 78
   - Sample SD = 5
   - Sample size = 25
   - $t = \frac{78 - 75}{5/\sqrt{25}} = 3$

5. **Critical Value**
   - $t_{0.05,24} = 1.711$ (one-tailed)

6. **Decision**
   - $t = 3 > 1.711$
   - Reject $H_0$

7. **Conclusion**
   - "The new teaching method significantly improves test scores (p < 0.05)"

## Related Topics
- [[Academic/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]]
- [[Academic/Statistics/Type I and Type II Errors\|Type I and Type II Errors]]
- [[Statistical Power\|Statistical Power]]
- [[P-values\|P-values]]
- [[Confidence Intervals\|Confidence Intervals]]
