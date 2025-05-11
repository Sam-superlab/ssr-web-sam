---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Basics/"}
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
| **Purpose**       | Formal statistical technique to answer binary questions (yes/no) about a [[Mainfolder/Statistics/Population\|Population]] using [[Mainfolder/Statistics/sample\|sample]] data |
| **Contrast with** | [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - which estimates parameters or provides ranges of plausible values                   |
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
| 3 | Calculate Test Statistic | * Compute sample statistic<br>* Standardize using [[Mainfolder/Statistics/Standard error\|Standard error]]<br>* Account for [[Mainfolder/Statistics/degrees of freedom\|degrees of freedom]] if needed |
| 4 | Determine P-value | * Identify [[Mainfolder/Statistics/sampling distribution\|sampling distribution]]<br>* Calculate probability of more extreme results<br>* Consider test direction (one/two-tailed) |
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
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Detailed explanation of null distribution, test statistics, and p-values
* [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Specific tests for population proportions
* [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Specific tests for population means
* [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Understanding the theoretical foundation for hypothesis testing
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Alternative approach to statistical inference
* [[Mainfolder/Statistics/Type I and Type II Errors\|Type I and Type II Errors]] - Understanding potential errors in hypothesis testing
* [[Mainfolder/Statistics/Statistical Significance\|Statistical Significance]] - Understanding what makes results significant 

## Comprehensive Guide to Hypothesis Tests

Below is a comprehensive overview of common hypothesis tests and when to use them:

| Category | Test | Use when … | Typical assumptions | Concrete scenario |
|----------|------|------------|---------------------|-------------------|
| **Single‑sample, one parameter** | **One‑sample $t$** | You have $\geq$ 1 quantitative measurement per subject and want to test $\mu = \mu_0$. | SRS/independence; population roughly normal or $n \geq 30$. | A dietitian records the daily sodium intake (mg) of 40 adults and asks if the mean differs from the CDC guideline of 2300 mg. |
| | **One‑sample $z$** | Same as above **but** $\sigma$ (population SD) is known (rare in practice). | SRS; quantitative; known $\sigma$. | A manufacturer knows the historical SD of bolt lengths is 0.2 mm and checks if a new machine's mean length = 20 mm using 50 bolts. |
| | **Sign / Wilcoxon signed‑rank** | Same goal as one‑sample $t$ but data are strongly non‑normal or ordinal. | Symmetry (signed‑rank); independence. | A small class ($n = 10$) rates instructor effectiveness on a 1–5 scale; instructor asks if the median differs from 3. |
| **Two paired measurements** | **Paired $t$** | Two quantitative measures on the *same* units (before–after, twin‑study, etc.). Test $\mu_d = 0$ for the *differences*. | Differences $\sim$ normal or $n \geq 30$. | Students take an R‐skills quiz pre‑ and post‑workshop; instructor tests if the mean improvement is $> 0$. |
| | **Wilcoxon signed‑rank (paired)** | Same as paired $t$ but non‑parametric. | Paired differences are symmetric. | Ten patients' pain scores (0–10) are measured before and after acupuncture; distribution is skewed. |
| **Two independent groups** | **Two‑sample $t$** | Compare means of a quantitative outcome across two independent groups. | Both groups $\sim$ normal (or $n \geq 30$); equal variances for pooled, or Welch for unequal. | Compare average exam scores for STEM vs Humanities majors. |
| | **Mann‑Whitney U (Wilcoxon rank‑sum)** | Same design as two‑sample $t$ but ordinal or non‑normal data. | Independent samples; similar shapes. | Median monthly rent of apartments in two cities using listings (skewed). |
| **$> 2$ independent groups** | **One‑way ANOVA** | Quantitative outcome, 1 categorical factor with $\geq 3$ groups; test equality of all group means. | Each group $\sim$ normal; equal variances; independence. | GPA compared across 1st‑, 2nd‑, 3rd‑, 4th‑year students. |
| | **Kruskal‑Wallis** | Non‑parametric alternative to one‑way ANOVA. | Independent samples; similar shapes. | Compare customer satisfaction (1–10 scale) for three delivery companies. |
| **Proportions & count data** | **One‑proportion $z$** | Binary outcome in one sample; test $p = p_0$. | $np$, $n(1-p) \geq 10$. | A poll of 200 voters asks if approval rate $= 0.50$. |
| | **Two‑proportion $z$** | Binary outcome, two indep. groups; test $p_1 = p_2$. | Counts in each group $\geq 10$ for success/failure. | Compare vaccine side‑effect rates in treatment vs placebo. |
| | **$\chi^2$ goodness‑of‑fit** | Single categorical variable with $k \geq 2$ levels; compare observed counts to a *specified* distribution. | Expected count per cell $\geq 5$. | Roll a die 120 times to check if it's fair (expected 20 per face). |
| | **$\chi^2$ test of independence ($k \times m$ table)** | Two categorical variables; test association (independence). | Expected counts $\geq 5$. | Sex (M/F) vs binge‑drinking (Yes/No) in a survey. |
| | **Fisher's exact** | Same design as $\chi^2$ independence but some expected counts $< 5$ or $n$ is small ($2 \times 2$ table). | None beyond independence. | 12 ICU patients: treatment vs control and survival (Yes/No). |
| **Correlation / association** | **Pearson correlation ($r$)** | Two *quantitative* variables; test $\rho = 0$. | Bivariate normality or roughly linear with no major outliers. | Height vs wingspan in basketball players. |
| | **Spearman rank correlation ($\rho_s$)** | Same goal, but variables ordinal or relationship monotone, not necessarily linear. | Continuous or ordinal; monotonic. | Daily rank of air‑quality index vs rank of traffic flow. |
| **Regression coefficients** | **Simple linear regression $t$‑test (slope)** | Quantitative $X \rightarrow$ quantitative $Y$; test $\beta_1 = 0$. | Linearity, independent errors, constant $\sigma$, normal errors. | Predict fuel efficiency from engine size. |
| | **Multiple regression partial $t$‑tests** | Several predictors; test a specific $\beta_j = 0$ controlling for others. | Same as above. | Predict salary from years‑experience, degree, and field. |
| **Variance / spread** | **$F$‑test for equal variances (2 groups)** | Want to decide if $\sigma_1^2 = \sigma_2^2$ (used less often nowadays). | Normality. | Compare variability in tensile strength from two suppliers. |
| | **Levene's / Brown–Forsythe** | Robust alternative to $F$‑test; uses absolute deviations. | Symmetric populations. | Test if three machines differ in variability of fill weight. | 