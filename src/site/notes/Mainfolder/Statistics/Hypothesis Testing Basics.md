---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Hypothesis Testing Basics/"}
---


## Introduction to Hypothesis Testing

*   **Purpose**: Hypothesis testing is a formal statistical technique used to answer binary questions (yes/no) about a [[Mainfolder/Statistics/Population\|Population]] using data collected from a [[Mainfolder/Statistics/sample\|sample]]. This contrasts with [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]], whose primary purpose is estimating a [[Mainfolder/Statistics/Parameter\|Parameter]] or providing a range of plausible values.
*   **Examples of Questions**:
    *   Is a coin fair? (yes/no)
    *   Is a new drug more effective than an existing one? (yes/no)
*   **Analogy (Court Case)**: Think of a court trial. We assume innocence (null hypothesis) until sufficient evidence suggests guilt (alternative hypothesis). Finding someone "not guilty" doesn't *prove* innocence, just that there wasn't enough evidence for guilt. Similarly, failing to reject the null hypothesis doesn't prove it's true.

### Core Components: The Hypotheses

Every hypothesis test involves two competing statements about a population parameter (e.g., population proportion $p$, population mean $\mu$).

| Component                      | Description                                                                                                         | Format                                                                                                                                                                      |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Null Hypothesis ($H_0$)        | Represents a skeptical viewpoint, the status quo, or an assumption of no effect, no difference, or no relationship. | $H_0: \text{parameter} = \text{hypothesized value}$                                                                                                                         |
| Alternative Hypothesis ($H_a$) | Represents what the researcher aims to find evidence *for*. It contradicts the null hypothesis.                     | $H_a: \text{parameter} > \text{value}$ (Right-tailed) <br> $H_a: \text{parameter} < \text{value}$ (Left-tailed) <br> $H_a: \text{parameter} \neq \text{value}$ (Two-tailed) |

### General Outline of a Hypothesis Test

| Step | Description                                                                                         |
| ---- | --------------------------------------------------------------------------------------------------- |
| 1    | Define Hypotheses: State $H_0$ and $H_a$ clearly in terms of the population parameter               |
| 2    | Simulate Under $H_0$ / Collect Data: Understand what [[Mainfolder/Statistics/sampling distribution\|sampling distribution]] look like if $H_0$ were true |
| 3    | Compare Statistic to Null: Calculate a test statistic                                               |
| 4    | Compute P-value: Calculate the probability of observing a test statistic as extreme or more extreme |
| 5    | Interpret/Conclude: Based on the p-value, decide whether to reject $H_0$                            |

### Related Topics
* [[Mainfolder/Statistics/Hypothesis Testing Key Concepts\|Hypothesis Testing Key Concepts]] - Detailed explanation of null distribution, test statistics, and p-values
* [[Mainfolder/Statistics/Hypothesis Testing for Proportions\|Hypothesis Testing for Proportions]] - Specific tests for population proportions
* [[Mainfolder/Statistics/Hypothesis Testing for Means\|Hypothesis Testing for Means]] - Specific tests for population means
* [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] - Understanding the theoretical foundation for hypothesis testing
* [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]] - Alternative approach to statistical inference 