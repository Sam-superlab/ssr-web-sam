---
{"dg-publish":true,"permalink":"/Academic/Statistics/ANOVA/"}
---

# Analysis of Variance (ANOVA)

## 1. Introduction

ANOVA is a collection of statistical models used to analyze differences among the means of multiple groups. The primary goal is to determine if there is a statistically significant difference between the means of two or more groups.

### Purpose and Focus

1. **Primary Purpose**
   * Test for differences among multiple group means
   * Evaluate if observed differences are statistically significant
   * Provide a framework for comparing more than two groups

2. **Key Focus Areas**
   * Overall group differences
   * Relative importance of different sources of variation
   * Statistical significance of group effects
   * Practical importance of differences

## 2. Hypotheses

ANOVA tests the following hypotheses regarding the means (μ) of *k* different groups:

- **Null Hypothesis (H₀)**: μ₁ = μ₂ = · · · = μₖ (All group means are equal)
  - Represents the "status quo" or assumption of no effect
- **Alternative Hypothesis (Hₐ)**: At least one μᵢ ≠ μⱼ (At least one group mean is different from the others)

## 3. The Core Idea: Partitioning Variance

Although ANOVA tests for differences in means, it does so by analyzing [[Academic/Statistics/Variance\|Variance]]. The fundamental idea is that the total variability in a dataset can be broken down into two components:

1. Variability within each group (also called error or residual variability)
2. Variability between the groups

The [[Academic/Statistics/F-distribution\|F-statistic]] compares the magnitude of these two sources of variability.

### Rationale for Using Variance

1. **Why Variance Instead of Means Directly**
   * Variance provides a measure of spread that's sensitive to differences
   * Allows comparison of group differences relative to within-group variation
   * Provides a standardized way to assess differences

2. **Advantages of Variance Analysis**
   * Handles multiple groups efficiently
   * Controls Type I error rate
   * Provides a single, comprehensive test
   * Allows for post-hoc analysis

## 4. Key Components and Calculations

### Sums of Squares

| Component                           | Formula                                                                 | Description                           |
| ----------------------------------- | ----------------------------------------------------------------------- | ------------------------------------- |
| Total Sum of Squares (SST)          | $SST = \sum_{all i,j} (x_{ij} - \bar{x})^2$                             | Total variability around overall mean |
| Sum of Squares Between Groups (SSG) | $SSG = \sum n_i (\bar{x}_i - \bar{x})^2$                                | Variability between group means       |
| Sum of Squared Errors (SSE)         | $SSE = \sum_{all i,j} (x_{ij} - \bar{x}_i)^2$ or $\sum (n_i - 1) s_i^2$ | Variability within groups             |

### Degrees of Freedom

| Source | Formula | Description |
|--------|---------|-------------|
| Group (Between) | $df = k - 1$ | Number of groups minus 1 |
| Error (Within) | $df = n - k$ | Total observations minus number of groups |
| Total | $df = n - 1$ | Total observations minus 1 |

### Mean Squares

| Component | Formula | Description |
|-----------|---------|-------------|
| Mean Square Groups (MSG) | $MSG = \frac{SSG}{k - 1}$ | Average between-group variance |
| Mean Square Error (MSE) | $MSE = \frac{SSE}{n - k}$ | Pooled within-group variance |

## 5. The F-statistic

The test statistic for ANOVA is the F-statistic:

$$
F = \frac{MSG}{MSE} = \frac{\text{Between-group Variation}}{\text{Within-group Variation (Error)}}
$$

A large F-statistic suggests that the variability between groups is large relative to the variability within groups, providing evidence against the null hypothesis.

### Interpretation of F-statistic

1. **Large F-value**
   * Indicates strong evidence against H₀
   * Suggests significant differences between groups
   * Relative to within-group variation

2. **F-value close to 1**
   * Suggests group means are similar
   * Provides weak evidence against H₀
   * Indicates within-group variation dominates

## 6. F Distribution and p-value

- The F-statistic follows an [[Academic/Statistics/F-distribution\|F-distribution]] with (k-1, n-k) degrees of freedom
- The p-value represents the probability of observing an F-statistic as large as or larger than the calculated value, assuming H₀ is true
- A small p-value (< 0.05) indicates strong evidence against H₀

## 7. ANOVA Table

| Source | df | Sum Sq | Mean Sq | F value | Pr(>F) |
|--------|----|--------|---------|---------|--------|
| Group | k-1 | SSG | MSG | F | p-value |
| Error | n-k | SSE | MSE | | |
| Total | n-1 | SST | | | |

## 8. Assumptions

For reliable ANOVA results, the following assumptions should be met:

1. [[Academic/Statistics/Normal Distribution\|Normality]]: Observations within each group should be approximately normally distributed
2. [[Academic/Statistics/Variance\|Homogeneity of Variance]]: Group variances should be approximately equal
3. [[Academic/Statistics/Independence\|Independence]]: Observations must be independent

### Checking Assumptions

1. **Normality**
   * Use normal probability plots
   * Consider sample size (n ≥ 30 often sufficient)
   * Check for skewness and outliers

2. **Homogeneity of Variance**
   * Levene's test
   * Bartlett's test
   * Visual inspection of group spreads

3. **Independence**
   * Consider study design
   * Check for repeated measures
   * Evaluate sampling method

## 9. Why Not Multiple t-tests?

- Multiple t-tests inflate the overall [[Academic/Statistics/Type I Error\|Type I error rate]]
- ANOVA performs a single test to evaluate all means simultaneously, controlling the overall error rate

### Multiple Testing Problem

1. **Error Rate Inflation**
   * Each test has α probability of Type I error
   * Multiple tests increase overall error rate
   * Family-wise error rate grows with number of tests

2. **ANOVA Solution**
   * Single test controls overall error rate
   * More powerful than multiple t-tests
   * Provides framework for post-hoc analysis

## 10. Post-Hoc Tests

If ANOVA is significant, post-hoc tests (e.g., [[Tukey HSD\|Tukey's HSD]]) can identify which specific group means differ while controlling the overall error rate.

### Common Post-Hoc Methods

1. **Tukey's HSD**
   * Controls family-wise error rate
   * Performs all pairwise comparisons
   * Provides confidence intervals

2. **Other Methods**
   * Bonferroni correction
   * Scheffe's method
   * Fisher's LSD

## 11. Connection to Regression

ANOVA can be viewed as a special case of linear regression where:
* Predictor variables are categorical
* Response variable is quantitative
* F-statistic tests overall model significance
* Provides framework for more complex analyses

## Types of ANOVA

### One-way ANOVA
- Single factor with multiple levels
- Tests for differences among group means
- Example: Comparing test scores across different teaching methods

### Two-way ANOVA
- Two factors with potential interaction
- Tests main effects and interaction effects
- Example: Studying effect of both teaching method and class size on test scores

### MANOVA (Multivariate ANOVA)
- Multiple dependent variables
- Tests for differences across multiple response variables
- Example: Comparing both test scores and student satisfaction across teaching methods

### Repeated Measures ANOVA
- Same subjects measured multiple times
- Accounts for within-subject correlation
- Example: Measuring student performance before, during, and after a teaching intervention

### Post-hoc Tests

When ANOVA indicates significant differences, post-hoc tests help identify which specific groups differ:

1. **Tukey's HSD (Honestly Significant Difference)**
   - Controls family-wise error rate
   - Performs all pairwise comparisons
   - Provides confidence intervals

2. **Bonferroni Correction**
   - Adjusts significance level for multiple comparisons
   - Conservative approach
   - Good for small number of comparisons

3. **Scheffé's Method**
   - Most conservative post-hoc test
   - Controls family-wise error rate
   - Good for complex comparisons

4. **Fisher's LSD (Least Significant Difference)**
   - Less conservative than others
   - Higher power but higher Type I error rate
   - Good for planned comparisons

### Connection to Regression

ANOVA can be viewed as a special case of regression where:
- Predictor variables are categorical
- Response variable is quantitative
- F-statistic tests overall model significance
- Provides framework for more complex analyses

## Related Topics
- [[Academic/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]]
- [[Academic/Statistics/t-distribution\|t-distribution]]
- [[Academic/Statistics/degrees of freedom\|degrees of freedom]]
- [[Academic/Statistics/Critical Values\|Critical Values]]
- [[Academic/Statistics/Confidence Interval\|Confidence Interval]]
- [[Academic/Statistics/Effect Size\|Effect Size]]
- [[Academic/Statistics/Power Analysis\|Power Analysis]]
- [[Multiple Comparisons\|Multiple Comparisons]]
- [[Academic/Statistics/Regression\|Regression]]
