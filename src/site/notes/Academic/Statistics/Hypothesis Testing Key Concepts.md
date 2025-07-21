---
{"dg-publish":true,"permalink":"/Academic/Statistics/Hypothesis Testing Key Concepts/"}
---

# Hypothesis Testing Key Concepts

## Purpose and Rationale

### Why These Concepts Matter
The key concepts in hypothesis testing serve several essential purposes:

1. **Understanding Test Mechanics**
   * Test statistics quantify the evidence against the null hypothesis
   * Null distributions provide the theoretical framework for decision-making
   * P-values measure the strength of evidence in a standardized way

2. **Making Valid Inferences**
   * Proper test selection ensures appropriate analysis
   * Understanding conditions ensures valid results
   * Error control helps manage decision risks

3. **Interpreting Results Correctly**
   * Clear framework for decision-making
   * Standardized way to communicate findings
   * Basis for comparing different studies

### The Rationale Behind Key Concepts

1. **Test Statistics**
   * Why we need them:
     * Standardize different types of evidence
     * Account for sample size and variability
     * Provide a common scale for comparison
     * Quantify deviation from null hypothesis
     * Simplify evaluation without full simulation
   * How they work:
     * Measure distance from null hypothesis
     * Account for sampling variability
     * Follow known probability distributions
     * Convert raw differences to standardized units
     * Enable probability calculations

2. **Null Distributions**
   * Why they're important:
     * Provide the theoretical basis for p-values
     * Help understand what to expect by chance
     * Enable calculation of probabilities
     * Define what constitutes "extreme" results
     * Allow for standardized decision making
   * How they're used:
     * Define what "extreme" means
     * Determine critical values
     * Calculate p-values
     * Guide test statistic interpretation
     * Support decision making

3. **Error Control**
   * Why it matters:
     * Helps manage decision risks
     * Provides framework for sample size planning
     * Enables comparison of different studies
     * Balances Type I and Type II errors
     * Guides practical decision making
   * How it works:
     * Balances Type I and Type II errors
     * Considers practical consequences
     * Guides decision thresholds
     * Helps determine sample sizes
     * Supports risk management

## Test Selection Guide

| Question Type | Test to Use | Key Conditions |
|--------------|-------------|----------------|
| Single Mean | t-test or z-test | Normal data or $n \geq 30$ |
| Difference in Means | Two-sample t-test | Independent samples |
| Single Proportion | z-test | $np_0 \geq 10$, $n(1-p_0) \geq 10$ |
| Difference in Proportions | Two-proportion z-test | Independent samples |

## Test Statistics and Evidence

### Purpose of Test Statistics

| Aspect | Description | Importance |
|--------|-------------|------------|
| Standardization | Converts raw differences to common scale | Enables comparison across studies |
| Evidence Quantification | Measures strength of evidence against H₀ | Provides objective basis for decisions |
| Variability Accounting | Incorporates sample size and spread | Ensures valid inference |
| Distribution Basis | Links to known probability distributions | Enables p-value calculation |

### Understanding P-values

| Concept | Description | Key Points |
|---------|-------------|------------|
| Definition | Probability of more extreme results under H₀ | *Not* probability H₀ is true |
| Interpretation | Strength of evidence against H₀ | Smaller p-value = stronger evidence |
| Calculation | Based on test statistic and null distribution | Depends on Hₐ direction |
| Usage | Two approaches: | 1. Strength of evidence<br>2. Decision making |

### P-value Interpretation Framework

| Approach | Method | When to Use |
|----------|--------|------------|
| Strength of Evidence | Direct p-value interpretation | Research reporting |
| Decision Making | Compare to α level | Practical applications |

### P-value Guidelines

| P-value Range | Traditional Interpretation | Better Practice |
|---------------|---------------------------|----------------|
| $p < 0.01$ | Strong evidence | Report exact p-value |
| $0.01 \leq p < 0.05$ | Moderate evidence | Consider practical significance |
| $0.05 \leq p < 0.10$ | Weak evidence | Discuss uncertainty |
| $p \geq 0.10$ | No evidence | Note limitations |

### Common Misconceptions About P-values

| Misconception | Reality | Explanation |
|---------------|---------|-------------|
| P-value = probability H₀ is true | False | P-value assumes H₀ is true |
| P-value = probability of random chance | False | P-value is conditional on H₀ |
| Small p-value proves Hₐ | False | Only provides evidence against H₀ |
| Large p-value proves H₀ | False | Only indicates insufficient evidence |

### Anatomy of Test Statistics

| Type | Formula | When to Use | Null Distribution |
|------|---------|-------------|------------------|
| Z-statistic | $Z = \frac{\text{estimate} - \text{null value}}{\text{standard error}}$ | Large samples, known $\sigma$ | $N(0,1)$ |
| T-statistic | $T = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$ | Small samples or unknown $\sigma$ | $t(df)$ |

### Components of Test Statistics

| Component | Description | Importance |
|-----------|-------------|------------|
| Numerator | Distance between observed and null | Measures effect size |
| Denominator | [[Academic/Statistics/Standard error\|Standard error]] | Measures precision |
| Absolute Value | Distance from zero | Strength of evidence |

### Null Distribution Properties

| Distribution | Used For | Key Features |
|--------------|----------|--------------|
| [[Academic/Statistics/Normal Distribution\|Normal Distribution]] | Large samples, proportions | Symmetric, uses z-scores |
| [[Academic/Statistics/t-distribution\|t-distribution]] | Small samples, means | Heavier tails, uses df |

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

## Best Practices

### Reporting Checklist

| Component | What to Include | Why Important |
|-----------|----------------|---------------|
| Hypotheses | Clear $H_0$ and $H_a$ | Defines research question |
| Conditions | All assumptions checked | Validates test choice |
| Test Statistic | Formula and calculation | Shows process |
| P-value | Exact value | Indicates evidence strength |
| Effect Size | Practical difference | Shows practical significance |
| [[Academic/Statistics/Confidence Interval\|Confidence Interval]] | Range estimate | Shows precision |

### Common Pitfalls to Avoid

| Pitfall | Consequence | Prevention |
|---------|-------------|------------|
| Multiple Testing | Increased Type I error | Adjust $\alpha$ level |
| P-hacking | Invalid conclusions | Pre-specify analyses |
| Binary Decisions | Loss of information | Report effect sizes |
| Ignoring Assumptions | Invalid results | Check conditions |

## Related Topics
- [[Academic/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction and overview
- [[Academic/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Tests for population means
- [[Academic/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Tests for population proportions
- [[Academic/Statistics/Critical Values\|Critical Values]] - Alternative to p-values
- [[Academic/Statistics/Standard error\|Standard error]] - Measure of estimate precision
- [[Academic/Statistics/sampling distribution\|sampling distribution]] - Foundation for hypothesis tests 