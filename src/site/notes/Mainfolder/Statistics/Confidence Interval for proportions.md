---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Confidence Interval for proportions/"}
---

## For a Single Population Proportion:

### 1. Parameter of Interest
| Type | Symbol | Description |
|------|---------|------------|
| Population Proportion | $p$ | The true proportion you're estimating |
| Sample Proportion | $\hat{p}$ | Number of successes / sample size |

### 2. Check Conditions
| Condition | Requirement | How to Check |
|-----------|-------------|--------------|
| Random Sample | Sample randomly selected | State whether met |
| Success Condition | $n \times \hat{p} \geq 10$ | Calculate and verify |
| Failure Condition | $n \times (1-\hat{p}) \geq 10$ | Calculate and verify |

### 3. Calculate Sample Proportion
$$\hat{p} = \frac{\text{number of successes}}{n}$$

### 4. Standard Error
Find in [[Mainfolder/Statistics/Standard error\|standard error]], but for proportion:
$$SE = \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$

### 5. Critical Values
| Confidence Level | $z^*$ Value |
|-----------------|-------------|
| 80% | 1.282 |
| 90% | 1.645 |
| 95% | 1.96 |
| 99% | 2.576 |

### 6. Confidence Interval Formula
$$\hat{p} \pm z^* \times SE$$

### 7. Interpretation Template
> "We are [confidence level]% confident that the true population proportion is between [lower bound] and [upper bound]."

## For Difference in Population Proportions:

### 1. Check Conditions
| Condition | Requirement | Notes |
|-----------|-------------|-------|
| Random Samples | Both groups randomly sampled | Essential for inference |
| Independence | Groups must be independent | No overlap between groups |
| Success/Failure | Check for both groups | All must be $\geq 10$ |

### 2. Calculations

#### Standard Error
Find in [[Mainfolder/Statistics/Standard error\|standard error]], but for difference in proportions:
$$SE = \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$

#### Confidence Interval
$$(\hat{p}_1 - \hat{p}_2) \pm z^* \times SE$$

### 3. Interpretation Guide
| Result | Interpretation |
|--------|---------------|
| Positive Interval | $p_1$ likely larger than $p_2$ |
| Negative Interval | $p_1$ likely smaller than $p_2$ |
| Contains Zero | No significant difference detected |

### Quick Reference Table
| Component | Single Proportion | Difference in Proportions |
|-----------|------------------|-------------------------|
| Point Estimate | $\hat{p}$ | $\hat{p}_1 - \hat{p}_2$ |
| Standard Error | $\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ | $\sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$ |
| Critical Value | $z^*$ | $z^*$ |
| Conditions | $n\hat{p} \geq 10$ and $n(1-\hat{p}) \geq 10$ | Check both groups separately |
