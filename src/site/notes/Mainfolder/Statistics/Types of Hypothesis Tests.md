---
dg-publish: true
---

# Types of Hypothesis Tests

## Purpose and Rationale

### Why Understanding Test Types Matters
Understanding different types of hypothesis tests is crucial because:

1. **Appropriate Test Selection**
   * Ensures valid statistical analysis
   * Prevents incorrect conclusions
   * Maximizes statistical power

2. **Research Design**
   * Guides data collection methods
   * Influences sample size planning
   * Affects study feasibility

3. **Result Interpretation**
   * Ensures correct p-value calculation
   * Guides proper decision making
   * Affects confidence in conclusions

### The Rationale Behind Test Selection

1. **Why We Need Different Tests**
   * Different data types require different approaches
   * Various research questions need specific methods
   * Statistical assumptions vary by test type

2. **How Test Selection Works**
   * Based on variable types
   * Depends on number of groups
   * Considers parameter of interest
   * Accounts for available information

## Test Selection Framework

### Key Factors to Consider

1. **Type of Variable**
   * Quantitative (numerical)
     - Testing means ($\mu$)
     - Examples: height, weight, price
   * Categorical (groups/categories)
     - Testing proportions ($p$)
     - Examples: yes/no, success/failure

2. **Number of Groups**
   * Single population
     - One-sample tests
   * Two populations
     - Two-sample tests
   * Multiple populations
     - ANOVA or multiple comparison tests

3. **Parameter of Interest**
   * Single quantitative: Population mean ($\mu$)
   * Two quantitative: Difference in means ($\mu_1 - \mu_2$)
   * Single categorical: Population proportion ($p$)
   * Two categorical: Difference in proportions ($p_1 - p_2$)

4. **Knowledge of Population Parameters**
   * Known $\sigma$: Z-tests
   * Unknown $\sigma$: T-tests

## Specific Test Types

### Tests for Proportions

1. **Single Proportion Test**
   * Hypotheses: $H_0: p = p_0$ vs $H_a: p [<, >, \neq] p_0$
   * Test Statistic: $Z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$
   * Distribution: Standard Normal, $N(0,1)$
   * Conditions:
     - Random sample
     - $np_0 \geq 10$ and $n(1-p_0) \geq 10$

2. **Difference in Proportions Test**
   * Hypotheses: $H_0: p_1 - p_2 = 0$ vs $H_a: p_1 - p_2 [<, >, \neq] 0$
   * Test Statistic: $Z = \frac{\hat{p}_1 - \hat{p}_2}{\sqrt{\hat{p}_{pool}(1-\hat{p}_{pool})(\frac{1}{n_1} + \frac{1}{n_2})}}$
   * Where $\hat{p}_{pool} = \frac{x_1 + x_2}{n_1 + n_2}$
   * Conditions:
     - Independent random samples
     - $n_1\hat{p}_1 \geq 10$, $n_1(1-\hat{p}_1) \geq 10$
     - $n_2\hat{p}_2 \geq 10$, $n_2(1-\hat{p}_2) \geq 10$

### Tests for Means

1. **Single Mean Test**
   * Hypotheses: $H_0: \mu = \mu_0$ vs $H_a: \mu [<, >, \neq] \mu_0$
   * Conditions:
     - Random sample
     - Normal population OR $n \geq 30$
   * Known $\sigma$:
     - Test Statistic: $Z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}$
     - Distribution: $N(0,1)$
   * Unknown $\sigma$:
     - Test Statistic: $T = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$
     - Distribution: $t$ with $df = n-1$

2. **Difference in Means Test**
   * Hypotheses: $H_0: \mu_1 - \mu_2 = 0$ vs $H_a: \mu_1 - \mu_2 [<, >, \neq] 0$
   * Conditions:
     - Independent random samples
     - Normal populations OR $n_1, n_2 \geq 30$
   * Known $\sigma$:
     - Test Statistic: $Z = \frac{\bar{x}_1 - \bar{x}_2}{\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}}$
     - Distribution: $N(0,1)$
   * Unknown $\sigma$:
     - Test Statistic: $T = \frac{\bar{x}_1 - \bar{x}_2}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}$
     - Distribution: $t$ with $df = \min(n_1, n_2) - 1$

## Test Selection Guide

### Decision Table

| Variable Type | Groups | Parameter | $\sigma$ Known? | Test | Distribution |
|---------------|--------|-----------|-----------------|------|--------------|
| Categorical | Single | $p$ | N/A | Z-test | $N(0,1)$ |
| Categorical | Two | $p_1 - p_2$ | N/A | Z-test | $N(0,1)$ |
| Quantitative | Single | $\mu$ | Yes | Z-test | $N(0,1)$ |
| Quantitative | Single | $\mu$ | No | T-test | $t_{n-1}$ |
| Quantitative | Two | $\mu_1 - \mu_2$ | Yes | Z-test | $N(0,1)$ |
| Quantitative | Two | $\mu_1 - \mu_2$ | No | T-test | $t_{\min(n_1,n_2)-1}$ |

## Best Practices

### Test Selection Process

1. **Before Analysis**
   * Identify variable types
   * Determine number of groups
   * Check parameter knowledge
   * Verify conditions

2. **During Analysis**
   * Use correct test statistic
   * Apply proper distribution
   * Calculate accurate p-value
   * Check assumptions

3. **After Analysis**
   * Report test used
   * Justify selection
   * Document conditions
   * Interpret results

### Common Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Wrong test | Invalid results | Follow selection guide |
| Ignoring conditions | Unreliable results | Check all assumptions |
| Incorrect distribution | Wrong p-values | Verify test type |

## Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Foundation for understanding tests
* [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]] - Interpreting test results
* [[P-value\|P-value]] - Understanding test outcomes
* [[Mainfolder/Statistics/Type I and Type II Errors\|Type I and Type II Errors]] - Potential mistakes in testing
* [[Mainfolder/Statistics/Power Analysis\|Power Analysis]] - Planning for adequate power
* [[Mainfolder/Statistics/Sample Size\|Sample Size]] - Determining required sample size
* [[Mainfolder/Statistics/Effect Size\|Effect Size]] - Measuring practical importance
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Alternative to hypothesis testing
* [[Mainfolder/Statistics/ANOVA\|ANOVA]] - Testing multiple means
* [[Mainfolder/Statistics/Chi-Square Tests\|Chi-Square Tests]] - Testing categorical variables 