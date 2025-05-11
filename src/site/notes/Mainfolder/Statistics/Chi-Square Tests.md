---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Chi-Square Tests/"}
---


# Chi-Square Tests

## Purpose and Rationale

Chi-square tests are specifically designed for analyzing categorical variables by comparing observed frequency counts with expected counts derived from a null hypothesis. This comparison helps determine if discrepancies between observed and expected counts are statistically significant or likely due to random chance.

### Core Applications

1. **Goodness-of-Fit Test**
   * Tests single categorical variable
   * Compares observed distribution to theoretical model
   * Evaluates if sample data matches expected proportions

2. **Test of Independence**
   * Tests association between two categorical variables
   * Evaluates if variables are independent or dependent
   * Analyzes patterns in contingency tables

## Test Statistics and Calculations

### Fundamental Formula
The core calculation for both tests:
$\chi^2 = \sum_{i=1}^k \frac{(O_i - E_i)^2}{E_i}$

Where:
- $k$ = number of categories/cells
- $O_i$ = observed count
- $E_i$ = expected count under $H_0$

### Expected Counts Calculation

1. **Goodness-of-Fit Test**
   * $E_i = N \times p_i^{(0)}$
   * Where $N$ = total sample size
   * $p_i^{(0)}$ = proportion specified in $H_0$

2. **Test of Independence**
   * $E_{ij} = \frac{(Row\ Total_i \times Column\ Total_j)}{Grand\ Total}$
   * For each cell in contingency table

## Theoretical Foundation

### Chi-Square Distribution
* Arises from sum of squared standard normal variables
* If $Z \sim N(0,1)$, then $Z^2 \sim \chi^2_1$
* Shape determined by degrees of freedom:
  - Goodness-of-Fit: $df = k - 1$
  - Test of Independence: $df = (r-1)(c-1)$

### Hypothesis Testing

1. **Goodness-of-Fit**
   * $H_0$: Population proportions equal specified values
   * $H_a$: At least one proportion differs
   * Example: $H_0: p_1 = p_2 = p_3 = p_4 = p_5 = 0.2$

2. **Test of Independence**
   * $H_0$: Variables are independent
   * $H_a$: Variables are dependent

## Applications and Best Practices

### Common Uses
* Survey analysis and experimental design
* Quality control and process monitoring
* Pattern analysis in categorical data
* Distribution testing and model validation

### Key Considerations

1. **Before Analysis**
   * Verify categorical nature of variables
   * Check expected count requirements
   * Plan adequate sample size

2. **During Analysis**
   * Calculate expected counts
   * Verify all conditions met
   * Compute test statistic

3. **After Analysis**
   * Interpret p-value in context
   * Consider practical significance
   * Report findings with effect size

### Common Pitfalls

| Issue | Problem | Solution |
|-------|---------|----------|
| Small expected counts | Invalid test | Combine categories |
| Ignoring assumptions | Unreliable results | Check all conditions |
| Overinterpreting | False conclusions | Consider context |

## Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Foundation for understanding tests
* [[Mainfolder/Statistics/Types of Hypothesis Tests\|Types of Hypothesis Tests]] - Choosing appropriate test
* [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]] - Interpreting results
* [[P-value\|P-value]] - Understanding test outcomes
* [[Contingency Tables\|Contingency Tables]] - Analyzing categorical data
* [[Mainfolder/Statistics/degrees of freedom\|Degrees of Freedom]] - Understanding test parameters
* [[Mainfolder/Statistics/Effect Size\|Effect Size]] - Measuring practical importance
* [[Mainfolder/Statistics/Sample Size\|Sample Size]] - Planning adequate samples
* [[Multiple Comparisons\|Multiple Comparisons]] - Handling multiple tests
* [[Mainfolder/Statistics/ANOVA\|ANOVA]] - Alternative for multiple groups 