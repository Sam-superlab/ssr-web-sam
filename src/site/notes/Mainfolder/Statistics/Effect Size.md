---
dg-publish: true
---

# Effect Size

## Purpose and Rationale

### Why Effect Size Matters
Effect size is crucial because:

1. **Practical Significance**
   * Measures magnitude of relationships
   * Indicates real-world importance
   * Complements statistical significance

2. **Research Interpretation**
   * Provides context for findings
   * Helps compare across studies
   * Enables meta-analyses

3. **Study Planning**
   * Guides sample size decisions
   * Helps set realistic expectations
   * Informs power analysis

### The Rationale Behind Effect Size

1. **Why We Need It**
   * p-values don't measure importance
   * Sample size affects significance
   * Need standardized measures

2. **How It Works**
   * Quantifies relationship strength
   * Provides standardized metrics
   * Enables meaningful comparisons

## Types of Effect Sizes

### For Mean Differences

| Measure | Formula | When to Use |
|---------|---------|-------------|
| Cohen's d | $\frac{M_1 - M_2}{\sigma}$ | Comparing two means |
| Hedges' g | Adjusted d | Small samples |
| Glass's Δ | $\frac{M_1 - M_2}{\sigma_{control}}$ | Control group reference |

### For Correlations

| Measure | Description | When to Use |
|---------|-------------|-------------|
| Pearson's $r$ | Linear correlation | Continuous variables |
| Point-biserial | Binary-continuous | Binary vs continuous |
| Phi coefficient | Binary-binary | Two binary variables |

### For Proportions

| Measure | Description | When to Use |
|---------|-------------|-------------|
| Risk ratio | $\frac{p_1}{p_2}$ | Comparing risks |
| Odds ratio | $\frac{p_1/(1-p_1)}{p_2/(1-p_2)}$ | Case-control studies |
| Risk difference | $p_1 - p_2$ | Direct comparison |

## Interpretation Guidelines

### Standard Benchmarks

| Effect Size | Small | Medium | Large |
|-------------|-------|--------|-------|
| Cohen's $d$ | 0.2 | 0.5 | 0.8 |
| Pearson's $r$ | 0.1 | 0.3 | 0.5 |
| Odds ratio | 1.5 | 2.5 | 4.0 |

### Contextual Considerations

1. **Field-Specific Standards**
   * Different fields have different norms
   * Consider typical effects in area
   * Review literature benchmarks

2. **Practical Importance**
   * Clinical significance
   * Economic impact
   * Real-world relevance

## Calculation Methods

### For Different Study Designs

| Design | Common Measures | Considerations |
|--------|----------------|----------------|
| Between-subjects | Cohen's d, η² | Group independence |
| Within-subjects | Cohen's dz, r | Repeated measures |
| Mixed designs | Partial η² | Complex designs |

### Software Implementation

| Software | Function | Example |
|----------|----------|---------|
| R | cohens_d() | cohens_d(group1, group2) |
| Python | scipy.stats | effect_size() |
| SPSS | Analyze → Compare Means | Effect size options |

## Reporting Guidelines

### Essential Elements

1. **What to Report**
   * Effect size measure used
   * Value and confidence interval
   * Interpretation context
   * Comparison benchmarks

2. **How to Present**
   * Clear labeling
   * Consistent formatting
   * Appropriate precision
   * Visual aids when helpful

### Common Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Not reporting | Missing context | Always include |
| Wrong measure | Inappropriate comparison | Choose carefully |
| Poor interpretation | Misleading conclusions | Use benchmarks |

## Applications

### Research Planning

1. **Sample Size**
   * Power analysis
   * Resource allocation
   * Study design

2. **Meta-Analysis**
   * Study comparison
   * Effect aggregation
   * Publication bias assessment

### Clinical Practice

1. **Treatment Effects**
   * Intervention impact
   * Clinical significance
   * Patient outcomes

2. **Risk Assessment**
   * Risk quantification
   * Decision making
   * Policy implications

## Best Practices

### Selection Guidelines

1. **Choose Appropriate Measure**
   * Consider research question
   * Match study design
   * Account for variables

2. **Consider Limitations**
   * Sample size effects
   * Distribution assumptions
   * Measurement issues

### Interpretation Framework

1. **Statistical Context**
   * Compare to benchmarks
   * Consider confidence intervals
   * Account for variability

2. **Practical Context**
   * Field-specific standards
   * Real-world implications
   * Stakeholder needs

## Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Basics\|Hypothesis Testing Basics]] - Foundation for effect size
* [[Mainfolder/Statistics/Power Analysis\|Power Analysis]] - Using effect size in planning
* [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]] - Complement to effect size
* [[Mainfolder/Statistics/Sample Size\|Sample Size]] - Relationship to effect size
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Precision of effect estimates
* [[Meta-Analysis\|Meta-Analysis]] - Combining effect sizes
* [[P-value\|P-value]] - Different from effect size
* [[Mainfolder/Statistics/ANOVA\|ANOVA]] - Effect sizes in ANOVA
* [[Mainfolder/Statistics/Correlation\|Correlation]] - Effect size for relationships
* [[Mainfolder/Statistics/Regression\|Regression]] - Effect size in regression 