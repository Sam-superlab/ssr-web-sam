---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Key Concepts/"}
---


## Key Concepts in Hypothesis Testing

### Null Distribution

| Aspect | Description |
|--------|-------------|
| Definition | Distribution of sample statistics if $H_0$ were true |
| Purpose | Simulates the world under "no effect" assumption |
| Characteristics | - Center: Hypothesized value from $H_0$ <br> - Spread: Depends on [[Mainfolder/Statistics/Standard error\|Standard error]] under $H_0$ |
| Common Forms | [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] for means/proportions (under [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]]) |

### Test Statistic

| Component | Description |
|-----------|-------------|
| Purpose | Standardized value for comparing sample statistic to null distribution |
| Formula | $\frac{\text{Sample Statistic} - \text{Null Hypothesis Value}}{\text{Standard Error}}$ |
| Interpretation | Measures difference in terms of standard errors |
| Distribution | [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] or [[Mainfolder/Statistics/t-distribution\|t-distribution]] depending on test type |

### P-value

| Aspect | Description |
|--------|-------------|
| Definition | Probability of observing a statistic as extreme or more extreme than observed, assuming $H_0$ is true |
| Interpretation | <table><tr><td>Small p-value</td><td>Strong evidence against $H_0$</td></tr><tr><td>Large p-value</td><td>Weak or no evidence against $H_0$</td></tr></table> |
| Calculation | Depends on $H_a$: <br> - Right-tailed: Area to right of test statistic <br> - Left-tailed: Area to left of test statistic <br> - Two-tailed: Area in both tails |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Introduction to hypothesis testing
* [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Application of these concepts to proportion tests
* [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Application of these concepts to mean tests
* [[Mainfolder/Statistics/Critical Values\|Critical Values]] - Important values for making decisions in hypothesis testing
* [[Mainfolder/Statistics/Standard error\|Standard error]] - Understanding the denominator in test statistics
* [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] - Important concept for t-distribution tests
* [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] - Foundation for understanding null distributions
* [[Mainfolder/Statistics/Normal Distribution\|Normal Distribution]] - Common distribution for test statistics 