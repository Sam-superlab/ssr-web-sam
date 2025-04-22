---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Key Concepts/"}
---

# Hypothesis Testing Key Concepts

## Test Selection Guide

| Question Type | Test to Use | Key Conditions |
|--------------|-------------|----------------|
| Single Mean | t-test or z-test | Normal data or $n \geq 30$ |
| Difference in Means | Two-sample t-test | Independent samples |
| Single Proportion | z-test | $np_0 \geq 10$, $n(1-p_0) \geq 10$ |
| Difference in Proportions | Two-proportion z-test | Independent samples |

## Test Statistics and Evidence

### Anatomy of Test Statistics

| Type | Formula | When to Use | Null Distribution |
|------|---------|-------------|------------------|
| Z-statistic | $Z = \frac{\text{estimate} - \text{null value}}{\text{standard error}}$ | Large samples, known $\sigma$ | $N(0,1)$ |
| T-statistic | $T = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$ | Small samples or unknown $\sigma$ | $t(df)$ |

### Components of Test Statistics

| Component | Description | Importance |
|-----------|-------------|------------|
| Numerator | Distance between observed and null | Measures effect size |
| Denominator | [[Mainfolder/Statistics/Standard error\|Standard error]] | Measures precision |
| Absolute Value | Distance from zero | Strength of evidence |

### Null Distribution Properties

| Distribution | Used For | Key Features |
|--------------|----------|--------------|
| [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] | Large samples, proportions | Symmetric, uses z-scores |
| [[Mainfolder/Statistics/t-distribution\|t-distribution]] | Small samples, means | Heavier tails, uses df |

## Decision Making Framework

### Types of Errors

| Decision vs Reality | $H_0$ True | $H_0$ False |
|-------------------|------------|-------------|
| Reject $H_0$ | Type I Error ($\alpha$) | Correct Decision |
| Fail to reject $H_0$ | Correct Decision | Type II Error ($\beta$) |

### Error Control Parameters

| Parameter | Symbol | Typical Values | Meaning |
|-----------|--------|----------------|----------|
| Significance Level | $\alpha$ | 0.05, 0.01 | Type I error rate |
| Power | $1-\beta$ | 0.80, 0.90 | Correct rejection rate |
| Sample Size | $n$ | Varies | Affects both errors |

### P-value Guidelines

| P-value Range | Traditional Interpretation | Better Practice |
|---------------|---------------------------|----------------|
| $p < 0.01$ | Strong evidence | Report exact p-value |
| $0.01 \leq p < 0.05$ | Moderate evidence | Consider practical significance |
| $0.05 \leq p < 0.10$ | Weak evidence | Discuss uncertainty |
| $p \geq 0.10$ | No evidence | Note limitations |

## Best Practices

### Reporting Checklist

| Component | What to Include | Why Important |
|-----------|----------------|---------------|
| Hypotheses | Clear $H_0$ and $H_a$ | Defines research question |
| Conditions | All assumptions checked | Validates test choice |
| Test Statistic | Formula and calculation | Shows process |
| P-value | Exact value | Indicates evidence strength |
| Effect Size | Practical difference | Shows practical significance |
| [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] | Range estimate | Shows precision |

### Common Pitfalls to Avoid

| Pitfall | Consequence | Prevention |
|---------|-------------|------------|
| Multiple Testing | Increased Type I error | Adjust $\alpha$ level |
| P-hacking | Invalid conclusions | Pre-specify analyses |
| Binary Decisions | Loss of information | Report effect sizes |
| Ignoring Assumptions | Invalid results | Check conditions |

## Related Topics
- [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction and overview
- [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Tests for population means
- [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Tests for population proportions
- [[Mainfolder/Statistics/Critical Values\|Critical Values]] - Alternative to p-values
- [[Mainfolder/Statistics/Standard error\|Standard error]] - Measure of estimate precision
- [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] - Foundation for hypothesis tests 