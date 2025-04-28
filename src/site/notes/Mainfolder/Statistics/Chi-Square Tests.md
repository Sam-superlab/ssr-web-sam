---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Chi-Square Tests/"}
---


# Chi-Square (χ²) Tests

## 1. Introduction

Chi-Square (χ²) tests are statistical methods primarily used for analyzing [[Mainfolder/Statistics/Categorical Variable\|categorical data]]. They help determine:

- If observed frequencies differ significantly from expected frequencies (Goodness-of-Fit test)
- If there is a statistically significant [[Mainfolder/Statistics/Association\|association]] between two categorical variables (Test of Independence)

## 2. The Chi-Square Distribution

### Mathematical Foundation
The χ² distribution arises from the sum of squared, independent [[Mainfolder/Statistics/Normal Distribution\|standard normal variables]] ($Z$). If $X_1, X_2, ..., X_k$ are independent standard normal variables ($N(0, 1)$), then:

$$
\sum_{i=1}^k X_i^2 \sim \chi^2_k
$$

### Key Properties
| Property | Formula | Description |
|----------|---------|-------------|
| Mean | $\mu = k$ | Center of the distribution |
| Variance | $\sigma^2 = 2k$ | Spread of the distribution |
| [[Mainfolder/Statistics/degrees of freedom\|Degrees of Freedom]] | $df = k$ | Shape parameter of the distribution |

## 3. The Chi-Square Test Statistic

The core formula for the χ² test statistic:

$$
\chi^2 = \sum_{i=1}^k \frac{(Observed_i - Expected_i)^2}{Expected_i}
$$

Where:
- $k$ = number of categories
- $Observed_i$ = actual count in category i
- $Expected_i$ = expected count under [[Mainfolder/Statistics/Hypothesis Testing Basics\|null hypothesis]]

## 4. Types of Chi-Square Tests

### A. Goodness-of-Fit Test

#### Purpose
Tests how well observed frequency distribution fits a hypothesized distribution.

#### Hypotheses
- $H_0$: Observed proportions match expected proportions
- $H_A$: At least one proportion differs significantly

#### Example: Multiple Choice Exam
| Answer | Observed | Expected |
|--------|----------|----------|
| A | 6 | 5 |
| B | 7 | 5 |
| C | 6 | 5 |
| D | 2 | 5 |
| E | 4 | 5 |

#### Example: Coin Flips
| Heads | Observed | Expected |
|-------|----------|----------|
| 0 | 28 | 25 |
| 1 | 55 | 50 |
| 2 | 17 | 25 |

Calculation:
$$
\chi^2 = \frac{(28-25)^2}{25} + \frac{(55-50)^2}{50} + \frac{(17-25)^2}{25} = 3.42
$$

### B. Test of Independence

#### Purpose
Tests [[Mainfolder/Statistics/Association\|association]] between two categorical variables.

#### Hypotheses
- $H_0$: Variables are [[Mainfolder/Statistics/Conditional Probability and Independence\|independent]]
- $H_A$: Variables are dependent

#### Expected Counts Formula
$$
Expected = \frac{(\text{Row Total}) \times (\text{Column Total})}{\text{Grand Total}}
$$

## 5. Interpreting Results

### P-value Interpretation
| P-value Range | Conclusion | Action |
|---------------|------------|--------|
| p < 0.05 | Strong evidence against H₀ | Reject H₀ |
| p ≥ 0.05 | Weak evidence against H₀ | Fail to reject H₀ |

See also: [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Concepts]]

## 6. Pros and Cons

### Advantages
- Versatile for comparing proportions across multiple groups
- Applicable to any number of categories (k ≥ 2)

### Limitations
- Only tests non-directional hypotheses
- Cannot directly test directional alternatives

## 7. R Implementation

### Goodness-of-Fit Example
```R
# Example: Multiple Choice Exam
obs <- c(6, 7, 6, 2, 4)
chisq.test(obs, p = c(0.2, 0.2, 0.2, 0.2, 0.2))

# Output:
# Chi-squared test for given probabilities
# data: obs
# X-squared = 3.2, df = 4, p-value = 0.5249
```

Interpretation: The high p-value (0.5249) indicates no significant deviation from expected distribution.

## Related Topics
- [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]]
- [[Mainfolder/Statistics/Probability Distributions\|Probability Distributions]]
- [[Mainfolder/Statistics/Critical Values\|Critical Values]]
- [[Mainfolder/Statistics/Tables\|Tables]] 