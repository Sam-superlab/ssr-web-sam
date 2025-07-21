---
{"dg-publish":true,"permalink":"/Academic/Statistics/Bootstrap/"}
---

## Introduction to Bootstrapping

Bootstrapping is a distribution-free approach that serves as an alternative to normal and t-distribution methods for statistical inference. Bootstrapping addresses a core challenge:

> "How to construct confidence intervals for non-mean/proportion statistics where CLT doesn't apply?"

## Fundamental Concept

Bootstrapping uses the original sample as a population proxy to create multiple resamples. The process follows:

| Step               | Description                                            |
| ------------------ | ------------------------------------------------------ |
| 1. Original Sample | Use sample as proxy population                         |
| 2. Resampling      | Create bootstrap samples with replacement              |
| 3. Sample Size     | Maintain original $n$ in each resample                 |
| 4. Distribution    | Build bootstrap distribution from resampled statistics |

## Advantages of Bootstrapping

| Advantage | Description |
|-----------|-------------|
| Distribution-free | No normality assumption required |
| Versatility | Works with various statistics beyond means and proportions |
| Flexibility | Handles medians, standard deviations, IQR |
| Minimal Assumptions | Requires fewer theoretical assumptions |

## Implementation Process

1. Create multiple bootstrap samples (typically $n \geq 1,000$ resamples)
2. Calculate the statistic of interest ($\theta^*$) for each resample
3. Aggregate results into a distribution plot
4. Observe the emergent distribution shape (often normal-like)
5. Identify the central peak around the original sample statistic ($\hat{\theta}$)

## Confidence Interval Derivation

### Percentile Method

| Confidence Level | Lower Bound | Upper Bound |
|-----------------|-------------|-------------|
| 95% CI | $2.5^{th}$ percentile | $97.5^{th}$ percentile |
| 90% CI | $5^{th}$ percentile | $95^{th}$ percentile |
| 99% CI | $0.5^{th}$ percentile | $99.5^{th}$ percentile |

### General Formula
For confidence level $(1-\alpha)$:
- Lower bound: $(\frac{\alpha}{2} \times 100)^{th}$ percentile
- Upper bound: $(1 - \frac{\alpha}{2} \times 100)^{th}$ percentile

## Critical Implementation Requirements

### 1. Data Requirements
| Requirement | Specification             |     |
| ----------- | ------------------------- | --- |
| Sampling    | Random selection required |     |
| Sample Size | $n \geq 30$ recommended   |     |

### 2. Resampling Protocol
- Strict replacement policy
- Maintain identical sample size
- Preserve original data values

### 3. Common Errors to Avoid
| Error | Why It's Problematic |
|-------|---------------------|
| No Replacement | Violates bootstrap principle |
| Changed Sample Size | Affects distribution properties |
| Modified Data | Introduces bias |

## Comparison to Traditional Methods

| Aspect | Traditional CI | Bootstrap CI |
|--------|---------------|--------------|
| Theoretical Basis | CLT/Normal Theory | Empirical Resampling |
| Data Requirements | Large $n$ | Moderate $n$ |
| Computational Load | Low | High |
| Flexibility | Limited | High |
| Assumptions | More strict | More flexible |

## R Implementation Example

```R
bootstrap <- function(x, statistic, n = 1000L) {
  bs <- replicate(n, {
    sb <- sample(x, replace = TRUE)
    statistic(sb)
  })
  data.frame(Sample = seq_len(n), Statistic = bs)
}
```

### Function Components
| Component | Purpose |
|-----------|----------|
| `x` | Input data vector |
| `statistic` | Function to compute desired statistic |
| `n` | Number of bootstrap resamples |
| `replace = TRUE` | Ensures proper bootstrap sampling |

## Validation Process

### Distribution Checking
1. Verify bootstrap distribution shape
2. Check symmetry properties:
   - Symmetric: Standard error methods may be applicable
   - Asymmetric: Prefer percentile method

### Quality Metrics
| Metric               | Target                 |
| -------------------- | ---------------------- |
| Number of Resamples  | $\geq 1,000$           |
| Coverage Probability | Close to nominal level |
| Distribution Shape   | Smooth, well-defined   |
