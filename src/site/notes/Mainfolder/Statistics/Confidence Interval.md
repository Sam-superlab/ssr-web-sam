---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Confidence Interval/"}
---

- [[Confidence Interval for population mean\|Confidence Interval for population mean]]
- [[Confidence Interval for proportions\|Confidence Interval for proportions]]
- [[Confidence Interval for difference between groups\|Confidence Interval for difference between groups]]

# Constructing Confidence Intervals - Reference Guide

When asked to construct a confidence interval, you should follow these key steps:

## 1. Identify what you're estimating
- Population mean ($\mu$): For quantitative variables like height, weight, scores
- Population proportion ($p$): For categorical variables (success/failure, yes/no)
- Difference between parameters: For comparing two groups

## 2. Check appropriate conditions
- For means:
  * Random sample
  * Either $n \geq 30$ OR population normally distributed
  
- For proportions:
  * Random sample
  * Success condition: $n \times \hat{p} \geq 10$
  * Failure condition: $n \times (1-\hat{p}) \geq 10$
  
- For differences:
  * Independent groups
  * Conditions for individual groups satisfied

## 3. Choose the appropriate formula
- For a mean: 

$$\bar{x} \pm t^* \times \frac{s}{\sqrt{n}}$$

- For a proportion: 

$$\hat{p} \pm z^* \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$

- For difference in means: 

$$(\bar{x}_1-\bar{x}_2) \pm t^* \times \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$$

- For difference in proportions: 

$$(\hat{p}_1-\hat{p}_2) \pm z^* \times \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$

## 4. Find critical value
- $z^*$ for proportions: Based on confidence level (e.g., 1.96 for 95%)
- $t^*$ for means: Based on confidence level and degrees of freedom $(n-1)$

## 5. Calculate margin of error
- Critical value × standard error

## 6. Construct interval
- Point estimate ± margin of error

## 7. Interpret result
"We are [confidence level]% confident that the true [parameter] lies between [lower bound] and [upper bound]."