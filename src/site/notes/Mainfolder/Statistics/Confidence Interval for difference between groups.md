---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Confidence Interval for difference between groups/"}
---

# Constructing Confidence Intervals: General Guidelines

When asked to construct a confidence interval, you should generally follow these steps:

## 1. Identify what you're estimating
- Is it a population mean (μ), proportion (p), or a difference between groups?
- Clearly define the parameter of interest in context of the problem

## 2. Check the conditions for creating a valid confidence interval
- For means:
  - Random sample
  - Either n ≥ 30 or the population is normally distributed
- For proportions:
  - Random sample
  - Success condition (n × p̂ ≥ 10)
  - Failure condition (n × (1-p̂) ≥ 10)
- For differences between groups:
  - Independence between groups
  - Plus the conditions for each individual group

## 3. Choose the appropriate formula
- For a mean: x̄ ± t* × (s/√n) using the t-distribution
- For a proportion: p̂ ± z* × √(p̂(1-p̂)/n) using the normal distribution
- For difference in means: (x̄₁ - x̄₂) ± t* × √(s₁²/n₁ + s₂²/n₂)
  - Note: df = min(n₁-1, n₂-1)
- For difference in proportions: (p̂₁ - p̂₂) ± z* × √(p̂₁(1-p̂₁)/n₁ + p̂₂(1-p̂₂)/n₂)

## 4. Find the critical value (z* or t*)
- For a specified confidence level (e.g., 95%), determine the appropriate critical value
- For proportions, use z* (e.g., 1.96 for 95% CI)
- For means with unknown σ, use t* with appropriate degrees of freedom (df = n-1)

## 5. Calculate the margin of error: critical value × standard error

## 6. Construct the interval: point estimate ± margin of error

## 7. Interpret the result
- "We are [confidence level]% confident that the true [parameter] is between [lower bound] and [upper bound]."
- For differences: specifically state which group was subtracted from which
- If interval contains 0 for a difference, note that no significant difference exists between groups
