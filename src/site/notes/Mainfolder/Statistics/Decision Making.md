---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Decision Making/"}
---


# Decision Making in Hypothesis Testing

Hypothesis testing offers a formal framework for answering binary questions using data. While one approach focuses on describing the strength of evidence against a null hypothesis ($H_0$), an alternative and historically common approach focuses on making a definitive decision.

## 1. The Core Decision

Based on the collected data and analysis, the ultimate goal in this approach is to make one of two decisions:

1. **Reject $H_0$**: There is sufficient evidence to reject the null hypothesis in favor of the alternative hypothesis ($H_a$). This suggests the observed data seems unlikely if $H_0$ were true.
2. **Fail to Reject $H_0$**: There is *not* sufficient evidence to reject the null hypothesis. This suggests the observed data largely agrees with $H_0$.

## 2. Potential Errors in Decision Making

Just like [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] can be correct or incorrect, decisions in hypothesis testing can also be wrong. There are two specific ways a decision can be incorrect:

### Type I Error
- **Definition**: Rejecting the null hypothesis ($H_0$) when $H_0$ is actually TRUE
- **Analogy**: A "False positive"
- **Example**: Concluding a new drug works when it actually doesn't
- **Rate**: Controlled by the significance level, denoted by $\alpha$ (alpha)

### Type II Error
- **Definition**: Failing to reject $H_0$ when $H_0$ is actually FALSE
- **Analogy**: A "False negative"
- **Example**: An effective drug is deemed ineffective
- **Rate**: Denoted by $\beta$ (beta)

### Summary Table of Decisions and Errors

| True State of Nature | Test Result          | $H_0$ True              | $H_0$ False             |
| :------------------- | :------------------- | :---------------------- | :---------------------- |
|                      | Fail to reject $H_0$ | Correct $(1-\alpha)$    | Type II Error $(\beta)$ |
|                      | Reject $H_0$         | Type I Error $(\alpha)$ | Correct $(1-\beta)$     |

## 3. Power

- **Definition**: Probability of *correctly* rejecting a false null hypothesis
- **Calculation**: Power = $1 - \beta$
- **Factors influencing power**:
  - Sample Size
  - Effect Size
  - Data Variability

## 4. The Decision Rule

The decision is made by comparing the calculated p-value to the pre-determined significance level ($\alpha$):
- If p-value $\leq \alpha$: Reject $H_0$
- If p-value $> \alpha$: Fail to reject $H_0$

## 5. Making Conclusions

A conclusion should typically include:
- The value of the test-statistic (e.g., Z or T) and the p-value
- A statement on whether $H_0$ is rejected or failed to be rejected
- An interpretation in the context of the original research question

## 6. Issues and Criticisms

### Arbitrary Significance Levels
- Common use of $\alpha = 0.05$ is historical convention
- Little practical difference between p-values slightly above or below 0.05

### Statistical vs. Practical Significance
- Rejecting $H_0$ indicates statistical significance
- Does not automatically mean practical significance
- Large sample sizes can make tiny differences statistically significant

### File Drawer Effect
- Research with "not significant" results may go unpublished
- Biases published literature towards positive results

### P-hacking
- Manipulating data or analysis to increase chance of significant p-value
- Techniques include:
  - Selectively removing outliers
  - Increasing sample size until significance is reached
  - Running many tests and only reporting significant ones

### Multiple Comparisons
- Conducting many hypothesis tests increases overall probability of Type I error
- If 8 independent tests at $\alpha = 0.05$, chance of at least one false positive $\approx 33.6\%$

## 7. Alternative Approach

Many statisticians increasingly favor the "strength of evidence" approach, which focuses on interpreting the p-value as a continuous measure of evidence against $H_0$ rather than making a strict reject/fail-to-reject decision based on an arbitrary $\alpha$ cutoff.

## Related Topics
- [[hypothesis testing\|Hypothesis Testing]]
- [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]]
- [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]]
- [[Mainfolder/Statistics/Type I and Type II Errors\|Type I and Type II Errors]]

