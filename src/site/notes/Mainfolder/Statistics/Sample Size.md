---
dg-publish: true
---

# Sample Size

## Purpose and Rationale

### Why Sample Size Matters
Sample size is crucial because:

1. **Statistical Power**
   * Affects ability to detect effects
   * Influences confidence in results
   * Determines study reliability

2. **Resource Management**
   * Impacts study costs
   * Affects time requirements
   * Influences feasibility

3. **Research Quality**
   * Affects precision of estimates
   * Influences generalizability
   * Impacts study validity

### The Rationale Behind Sample Size

1. **Why We Need It**
   * Too small: Miss important effects
   * Too large: Waste resources
   * Just right: Optimal balance

2. **How It Works**
   * Balances statistical needs
   * Considers practical constraints
   * Ensures adequate power

## Factors Affecting Sample Size

### Statistical Considerations

| Factor | Effect | How to Address |
|--------|--------|----------------|
| Effect size | Smaller effect = larger $n$ | Use realistic estimates |
| Power | Higher power = larger $n$ | Choose appropriate level |
| Significance | Lower $\alpha$ = larger $n$ | Set appropriate $\alpha$ |
| Variability | More variation = larger $n$ | Improve measurement |

### Practical Considerations

| Factor | Impact | Solution |
|--------|--------|----------|
| Resources | Limited budget | Optimize design |
| Time | Limited time | Plan efficiently |
| Population | Limited access | Consider alternatives |
| Ethics | Participant burden | Minimize n when possible |

## Calculation Methods

### For Different Study Designs

| Design | Formula | Considerations |
|--------|---------|----------------|
| One sample | $n = \frac{(Z_{\alpha/2} + Z_{\beta})^2\sigma^2}{\delta^2}$ | Single group |
| Two samples | $n = \frac{2(Z_{\alpha/2} + Z_{\beta})^2\sigma^2}{\delta^2}$ | Two groups |
| Paired samples | $n = \frac{(Z_{\alpha/2} + Z_{\beta})^2\sigma_d^2}{\delta^2}$ | Before-after |
| Proportions | $n = \frac{(Z_{\alpha/2} + Z_{\beta})^2p(1-p)}{\delta^2}$ | Binary outcomes |

### Software Tools

| Tool | Features | Best For |
|------|----------|----------|
| G*Power | Comprehensive | Most analyses |
| R packages | Flexible | Custom needs |
| Online calculators | Quick | Simple cases |

## Planning Process

### Step-by-Step Approach

1. **Define Parameters**
   * Expected effect size
   * Desired power
   * Significance level
   * Expected variability

2. **Consider Constraints**
   * Available resources
   * Time limitations
   * Population access
   * Ethical considerations

3. **Calculate Initial Size**
   * Use appropriate formula
   * Apply correction factors
   * Consider design effects

4. **Adjust as Needed**
   * Account for attrition
   * Consider clustering
   * Adjust for multiple tests
   * Round to practical number

## Common Scenarios

### Clinical Trials

| Phase | Considerations | Typical Size |
|-------|----------------|--------------|
| I | Safety | Small (20-80) |
| II | Efficacy | Medium (100-300) |
| III | Effectiveness | Large (300-3000) |
| IV | Post-marketing | Very large |

### Survey Research

| Type | Considerations | Typical Size |
|------|----------------|--------------|
| National | Representativeness | 1000+ |
| Regional | Local focus | 300-1000 |
| Specialized | Specific population | 100-500 |

## Best Practices

### Planning Guidelines

1. **Before Calculation**
   * Review literature
   * Consult experts
   * Consider alternatives
   * Document assumptions

2. **During Calculation**
   * Use conservative estimates
   * Consider multiple scenarios
   * Account for practicalities
   * Document process

3. **After Calculation**
   * Justify final size
   * Consider alternatives
   * Plan for contingencies
   * Document rationale

### Common Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Too small | Low power | Use power analysis |
| Too large | Waste resources | Consider costs |
| No justification | Poor planning | Document rationale |
| Ignoring constraints | Unrealistic | Consider limitations |

## Reporting Guidelines

### Essential Elements

1. **What to Report**
   * Calculation method
   * Assumptions made
   * Parameters used
   * Justification

2. **How to Present**
   * Clear explanation
   * Supporting rationale
   * Alternative considerations
   * Limitations

## Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Foundation for sample size
* [[Mainfolder/Statistics/Power Analysis\|Power Analysis]] - Determining required sample size
* [[Mainfolder/Statistics/Effect Size\|Effect Size]] - Impact on sample size
* [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]] - Relationship to sample size
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Precision and sample size
* [[Multiple Comparisons\|Multiple Comparisons]] - Adjusting sample size
* [[P-value\|P-value]] - Significance and sample size
* [[Mainfolder/Statistics/ANOVA\|ANOVA]] - Sample size for multiple groups
* [[Mainfolder/Statistics/Regression\|Regression]] - Sample size for models
* [[Survey Design\|Survey Design]] - Sample size for surveys 