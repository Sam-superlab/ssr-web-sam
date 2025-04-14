---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Basics/"}
---


## Introduction to Hypothesis Testing

| Aspect | Description |
|--------|-------------|
| **Purpose** | Formal statistical technique to answer binary questions (yes/no) about a [[Mainfolder/Statistics/Population\|Population]] using [[Mainfolder/Statistics/sample\|sample]] data |
| **Contrast with** | [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - which estimates parameters or provides ranges of plausible values |
| **Key Feature** | Compares two competing possibilities about a population parameter |

### Examples of Hypothesis Testing Questions

| Type | Example |
|------|---------|
| Fairness Test | Is a coin fair? (yes/no) |
| Treatment Effect | Is a new drug more effective than an existing one? (yes/no) |
| Quality Control | Does a manufacturing process meet specifications? (yes/no) |

### Court Case Analogy

| Concept | Court Case | Hypothesis Testing |
|---------|------------|-------------------|
| Initial Assumption | Innocence | Null Hypothesis ($H_0$) |
| Alternative | Guilt | Alternative Hypothesis ($H_a$) |
| Evidence Required | Beyond reasonable doubt | Small p-value |
| Decision | Not guilty ≠ innocent | Fail to reject $H_0$ ≠ $H_0$ is true |

### Core Components: The Hypotheses

| Component | Description | Format |
|-----------|-------------|--------|
| Null Hypothesis ($H_0$) | Represents skepticism, status quo, or no effect | $H_0: \text{parameter} = \text{hypothesized value}$ |
| Alternative Hypothesis ($H_a$) | Represents what we aim to find evidence for | $H_a: \text{parameter} > \text{value}$ (Right-tailed) <br> $H_a: \text{parameter} < \text{value}$ (Left-tailed) <br> $H_a: \text{parameter} \neq \text{value}$ (Two-tailed) |

### General Outline of a Hypothesis Test

| Step | Description | Key Components |
|------|-------------|----------------|
| 1 | Define Hypotheses | State $H_0$ and $H_a$ clearly |
| 2 | Simulate/Collect | Understand [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] under $H_0$ |
| 3 | Compare | Calculate test statistic |
| 4 | Compute | Calculate p-value |
| 5 | Interpret | Make decision based on p-value |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Detailed explanation of null distribution, test statistics, and p-values
* [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Specific tests for population proportions
* [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Specific tests for population means
* [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Understanding the theoretical foundation for hypothesis testing
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Alternative approach to statistical inference 