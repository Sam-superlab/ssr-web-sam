---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/ANOVA/"}
---

# Analysis of Variance (ANOVA)

## 1. Introduction

ANOVA is a collection of statistical models used to analyze differences among the means of multiple groups. The primary goal is to determine if there is a statistically significant difference between the means of two or more groups.

## 2. Hypotheses

ANOVA tests the following hypotheses regarding the means (μ) of *k* different groups:

- **Null Hypothesis (H₀)**: μ₁ = μ₂ = · · · = μₖ (All group means are equal)
  - Represents the "status quo" or assumption of no effect
- **Alternative Hypothesis (Hₐ)**: At least one μᵢ ≠ μⱼ (At least one group mean is different from the others)

## 3. The Core Idea: Partitioning Variance

Although ANOVA tests for differences in means, it does so by analyzing [[Mainfolder/Statistics/Variance\|Variance]]. The fundamental idea is that the total variability in a dataset can be broken down into two components:

1. Variability within each group (also called error or residual variability)
2. Variability between the groups

The [[Mainfolder/Statistics/F-distribution\|F-statistic]] compares the magnitude of these two sources of variability.

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

## 6. F Distribution and p-value

- The F-statistic follows an [[Mainfolder/Statistics/F-distribution\|F-distribution]] with (k-1, n-k) degrees of freedom
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

1. [[Mainfolder/Statistics/Normal Distribution\|Normality]]: Observations within each group should be approximately normally distributed
2. [[Mainfolder/Statistics/Variance\|Homogeneity of Variance]]: Group variances should be approximately equal
3. [[Mainfolder/Statistics/Independence\|Independence]]: Observations must be independent

## 9. Why Not Multiple t-tests?

- Multiple t-tests inflate the overall [[Mainfolder/Statistics/Type I Error\|Type I error rate]]
- ANOVA performs a single test to evaluate all means simultaneously, controlling the overall error rate

## 10. Post-Hoc Tests

If ANOVA is significant, post-hoc tests (e.g., [[Tukey HSD\|Tukey's HSD]]) can identify which specific group means differ while controlling the overall error rate.

## Related Topics
- [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]]
- [[Mainfolder/Statistics/t-distribution\|t-distribution]]
- [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]]
- [[Mainfolder/Statistics/Critical Values\|Critical Values]]
- [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]]
