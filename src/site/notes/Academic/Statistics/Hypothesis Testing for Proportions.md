---
{"dg-publish":true,"permalink":"/Academic/Statistics/Hypothesis Testing for Proportions/"}
---

# Hypothesis Tests for Proportions

## Test Selection Guide

| Test Type | When to Use | Key Conditions | Example |
|-----------|-------------|----------------|---------|
| Single Proportion | Compare to hypothesized value | $np_0 \geq 10$, $n(1-p_0) \geq 10$ | Testing if majority supports (p > 0.5) |
| Difference in Proportions | Compare two groups | All $n\hat{p} \geq 10$ | Comparing treatment success rates |

## Single Proportion Test

### Hypotheses Structure

| Type | Symbolic Form | Example |
|------|--------------|---------|
| Null | $H_0: p = p_0$ | $H_0: p = 0.5$ |
| Right-tailed | $H_a: p > p_0$ | $H_a: p > 0.5$ |
| Left-tailed | $H_a: p < p_0$ | $H_a: p < 0.5$ |
| Two-tailed | $H_a: p \neq p_0$ | $H_a: p \neq 0.5$ |

### Test Statistic Components

| Component | Formula/Value | Description |
|-----------|--------------|-------------|
| Statistic | $Z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$ | Test statistic |
| $\hat{p}$ | $\frac{\text{successes}}{n}$ | Sample proportion |
| $p_0$ | Hypothesized value | Null value |
| $n$ | Sample size | Number of observations |

### Conditions Checklist

| Condition | Requirement | How to Verify |
|-----------|-------------|---------------|
| Random Sample | Independent observations | Study design |
| Success-Failure | $np_0 \geq 10$ | Calculate $np_0$ |
| | $n(1-p_0) \geq 10$ | Calculate $n(1-p_0)$ |

### Distribution Properties

| Aspect | Details | Notes |
|--------|---------|-------|
| Type | Normal approximation | Based on [[Academic/Statistics/Central Limit Theorem\|Central Limit Theorem]] |
| Center | $p_0$ under $H_0$ | Null hypothesis value |
| Spread | $\sqrt{\frac{p_0(1-p_0)}{n}}$ | Standard error |

## Difference of Proportions Test

### Hypotheses Structure

| Type | Symbolic Form | Interpretation |
|------|--------------|----------------|
| Null | $H_0: p_1 - p_2 = 0$ | No difference |
| Alternative | $H_a: p_1 - p_2$ [<, >, ≠] $0$ | Difference exists |

### Test Statistic Components

| Component | Formula | Purpose |
|-----------|---------|---------|
| Pooled Proportion | $\hat{p} = \frac{x_1 + x_2}{n_1 + n_2}$ | Combined estimate under $H_0$ |
| Test Statistic | $Z = \frac{(\hat{p}_1 - \hat{p}_2)}{\sqrt{\hat{p}(1-\hat{p})(\frac{1}{n_1} + \frac{1}{n_2})}}$ | Standardized difference |

### Success-Failure Conditions

| Group | Conditions | Example Check |
|-------|------------|---------------|
| Group 1 | $n_1\hat{p} \geq 10$ | 100(0.5) = 50 ✓ |
| | $n_1(1-\hat{p}) \geq 10$ | 100(0.5) = 50 ✓ |
| Group 2 | $n_2\hat{p} \geq 10$ | 100(0.5) = 50 ✓ |
| | $n_2(1-\hat{p}) \geq 10$ | 100(0.5) = 50 ✓ |

### Common Applications

| Application | Example | Key Considerations |
|-------------|---------|-------------------|
| A/B Testing | Website conversion | Independence |
| Clinical Trials | Treatment success | Randomization |
| Survey Analysis | Response differences | Sample selection |
| Quality Control | Defect rates | Time independence |

## Best Practices

### Reporting Template

| Element | Content | Example |
|---------|---------|---------|
| Context | Research question | "Testing if new treatment improves success rate" |
| Method | Test type and conditions | "Two-proportion z-test, conditions met" |
| Results | Statistics and p-value | "z = 2.45, p = 0.014" |
| Conclusion | Interpretation | "Evidence suggests improvement of 12%" |

### Interpretation Guide

| Finding | Statistical Meaning | Practical Action |
|---------|-------------------|------------------|
| Significant Difference | Reject $H_0$ | Consider effect size |
| No Significant Difference | Fail to reject $H_0$ | Consider power |
| Large Effect | Practical importance | Implement changes |
| Small Effect | Statistical significance only | Consider costs |

## Related Topics
- [[Academic/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - General framework
- [[Academic/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Core concepts
- [[Academic/Statistics/Normal Distribution\|Normal Distribution]] - Key distribution for proportion tests
- [[Academic/Statistics/Standard error\|Standard error]] - Understanding uncertainty
- [[Academic/Statistics/Confidence Interval for proportions\|Confidence Interval for proportions]] - Complementary inference approach
- [[Academic/Statistics/sampling distribution\|sampling distribution]] - Foundation for tests 