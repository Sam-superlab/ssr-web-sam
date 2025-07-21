---
{"dg-publish":true,"permalink":"/Academic/Statistics/Hypothesis Testing Basics/"}
---


# Hypothesis Testing Basics

## Purpose and Rationale

### Why Do We Need Hypothesis Testing?
Hypothesis testing serves several crucial purposes in statistical analysis:

1. **Making Data-Driven Decisions**
   * Provides a structured framework for making decisions based on sample data
   * Helps avoid making decisions based on intuition or anecdotal evidence
   * Allows us to quantify the strength of evidence for or against a claim

2. **Scientific Method Application**
   * Enables systematic testing of theories and claims
   * Provides a way to falsify hypotheses (following Popper's philosophy)
   * Allows for replication and verification of results

3. **Risk Management**
   * Helps quantify the probability of making incorrect decisions
   * Provides a way to control Type I and Type II errors
   * Allows for setting acceptable levels of risk in decision-making

### The Rationale Behind Hypothesis Testing

1. **Statistical Inference**
   * We can't observe entire populations, so we use samples
   * Sample results vary due to random sampling
   * Need a method to distinguish between:
     * Real effects/patterns
     * Random variation in the data

2. **Burden of Proof**
   * Starts with a skeptical position (null hypothesis)
   * Requires strong evidence to reject the null
   * Protects against false discoveries
   * Similar to "innocent until proven guilty" in legal systems

3. **Quantifying Uncertainty**
   * Provides a way to measure the strength of evidence
   * Allows for comparison of different studies
   * Helps in making informed decisions under uncertainty

## Introduction to Hypothesis Testing

| Aspect            | Description                                                                                                   |
| ----------------- | ------------------------------------------------------------------------------------------------------------- |
| **Purpose**       | Formal statistical technique to answer binary questions (yes/no) about a [[Academic/Statistics/Population\|Population]] using [[Academic/Statistics/sample\|sample]] data |
| **Contrast with** | [[Academic/Statistics/Confidence Interval\|Confidence Interval]] - which estimates parameters or provides ranges of plausible values                   |
| **Key Feature**   | Compares two competing possibilities about a population parameter                                             |

### Examples of Hypothesis Testing Questions

| Type | Example |
|------|---------|
| Fairness Test | Is a coin fair? (yes/no) |
| Treatment Effect | Is a new drug more effective than an existing one? (yes/no) |
| Quality Control | Does a manufacturing process meet specifications? (yes/no) |
| Population Parameter | Is the mean height of a population different from a known value? |
| Relationship | Is there a relationship between two categorical variables? |

### Court Case Analogy

| Concept | Court Case | Hypothesis Testing |
|---------|------------|-------------------|
| Initial Assumption | Innocence | Null Hypothesis ($H_0$) |
| Alternative | Guilt | Alternative Hypothesis ($H_a$) |
| Evidence Required | Beyond reasonable doubt | Small p-value |
| Decision | Not guilty ≠ innocent | Fail to reject $H_0$ ≠ $H_0$ is true |
| Burden of Proof | On prosecution | On alternative hypothesis |

### Core Components: The Hypotheses

| Component | Description | Format |
|-----------|-------------|--------|
| Null Hypothesis ($H_0$) | Represents skepticism, status quo, or no effect | $H_0: \text{parameter} = \text{hypothesized value}$ |
| Alternative Hypothesis ($H_a$) | Represents what we aim to find evidence for | $H_a: \text{parameter} > \text{value}$ (Right-tailed) <br> $H_a: \text{parameter} < \text{value}$ (Left-tailed) <br> $H_a: \text{parameter} \neq \text{value}$ (Two-tailed) |

### Detailed Hypothesis Testing Procedure

| Step | Description | Key Components |
|------|-------------|----------------|
| 1 | Define Hypotheses | * State $H_0$ and $H_a$ clearly<br>* Choose appropriate test type<br>* Determine if one or two-tailed |
| 2 | Collect Data and Check Conditions | * Gather random sample(s)<br>* Verify sample size conditions<br>* Check distribution assumptions<br>* Ensure independence |
| 3 | Calculate Test Statistic | * Compute sample statistic<br>* Standardize using [[Academic/Statistics/Standard error\|Standard error]]<br>* Account for [[Academic/Statistics/degrees of freedom\|degrees of freedom]] if needed |
| 4 | Determine P-value | * Identify [[Academic/Statistics/sampling distribution\|sampling distribution]]<br>* Calculate probability of more extreme results<br>* Consider test direction (one/two-tailed) |
| 5 | Make Decision | * Compare p-value to significance level<br>* State conclusion in context<br>* Consider practical significance |

### Key Considerations

| Aspect | Description |
|--------|-------------|
| Sample Size | Affects power and validity of assumptions |
| Significance Level | Pre-determined threshold (often α = 0.05) |
| Test Direction | One-tailed vs two-tailed affects p-value calculation |
| Conditions | Must be verified for valid inference |
| Practical Significance | Statistical significance ≠ practical importance |

### Common Misconceptions

| Misconception | Reality |
|---------------|---------|
| "Fail to reject" means $H_0$ is true | It only means insufficient evidence to reject |
| Small p-value proves $H_a$ | It only provides evidence against $H_0$ |
| Large p-value proves $H_0$ | It only means insufficient evidence against $H_0$ |
| Statistical significance = practical importance | They are different concepts |

### Related Topics
* [[Academic/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Detailed explanation of null distribution, test statistics, and p-values
* [[Academic/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Specific tests for population proportions
* [[Academic/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Specific tests for population means
* [[Academic/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Understanding the theoretical foundation for hypothesis testing
* [[Academic/Statistics/Confidence Interval\|Confidence Interval]] - Alternative approach to statistical inference
* [[Academic/Statistics/Type I and Type II Errors\|Type I and Type II Errors]] - Understanding potential errors in hypothesis testing
* [[Academic/Statistics/Statistical Significance\|Statistical Significance]] - Understanding what makes results significant 

## Comprehensive Guide to Hypothesis Tests

| **Section / Term**                  | **What it refers to**                                                                                           | **How to interpret it**                                                                                                                                                                       | **Why it matters**                              |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| **Call**                            | Formula you passed to `lm()` (e.g. `Net_Tuition ~ Enrollment + Type`).                                           | Confirms the model you actually fit: response on the left, predictors on the right.                                                                                                            | Quick specification check                       |
| **Coefficients block**              | Estimates and tests for each parameter in $$\hat{Y}=b_0+b_1X_1+\dots+b_kX_k$$.                                   | —                                                                                                                                                                                             | —                                               |
| &nbsp;&nbsp;`Estimate`              | $\hat\beta_i$: best‑fit coefficient (intercept or slope).                                                        | **Slope:** expected change in *Y* for a 1‑unit rise in that predictor, holding others constant.<br>**Intercept:** predicted *Y* when all $X=0$ (if $X=0$ is meaningful).                      | Direction & magnitude of each relationship      |
| &nbsp;&nbsp;`Std. Error`            | $\text{SE}(\hat\beta_i)$: estimated SD of the sampling distribution of $\hat\beta_i$.                            | Smaller SE ⇒ more precise estimate.                                                                                                                                                           | Precision of estimate                           |
| &nbsp;&nbsp;`t value`               | \(t=\dfrac{\text{Estimate}}{\text{Std.Error}}\).                                                                 | Large \|t\| ⇒ estimate is many SEs from 0 ⇒ evidence that the true $\beta_i\neq0$.                                                                                                             | Test statistic for $H_0\!:\beta_i=0$            |
| &nbsp;&nbsp;`Pr(\>|t\|)`            | Two‑sided *p*‑value for that *t*‑test.                                                                           | If *p* \< α (e.g. 0.05), reject $H_0$: the predictor is statistically significant.                                                                                                             | Significance of each predictor                 |
| **Residual standard error**         | $\hat\sigma$: SD of residuals (units of *Y*).                                                                    | Typical prediction error; lower ⇒ tighter fit.                                                                                                                                                | Absolute measure of model accuracy             |
| **df (Residuals)**                  | $n-k-1$: observations minus parameters.                                                                         | Used in *t*‑ and *F*‑tests.                                                                                                                                                                   | Calibration of p‑values                        |
| **Multiple R‑squared**              | $R^2$: proportion of variance in *Y* explained by the predictors.                                               | Ranges 0–1; higher ⇒ stronger explanatory power.                                                                                                                                              | Strength of fit                                |
| **Adjusted R‑squared**              | $R^2$ adjusted for number of predictors.                                                                        | Penalises unnecessary predictors; use to compare models of different sizes.                                                                                                                   | Strength of fit (penalised)                    |
| **F‑statistic**                     | Tests \(H_0\!:\beta_1=\dots=\beta_k=0\) (no slopes).                                                             | Large *F* ⇒ at least one slope ≠ 0.                                                                                                                                                           | Overall model significance                     |
| &nbsp;&nbsp;`p‑value` (for *F*)     | Probability of that *F* (or larger) under \(H_0\).                                                              | *p* \< α ⇒ model is statistically useful overall.                                                                                                                                            | Global test of usefulness                      |
