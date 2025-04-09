---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/sampling distribution/"}
---

## Definition and Purpose
> A sampling distribution is the **distribution of statistics from many samples** (all with the same sample size)

## Understanding Dots in Sampling Distributions

Each dot in a sampling distribution for the mean represents a single sample mean ($\bar{x}$) calculated from one sample of size $n$. The position of the dot on the x-axis shows the value of that sample mean.

### How Dots Are Created
1. Take a random sample of size $n$ from the population
2. Calculate the mean ($\bar{x}$) for this sample
3. Plot this mean as one dot
4. Repeat many times with new samples of the same size

### What the Pattern Tells Us

The overall pattern of dots reveals important information about the sampling distribution:
- **Clustering**: Where dots cluster shows common sample mean values
- **Center**: The center of the dots approximates the population mean $\mu$
- **Spread**: The spread of dots shows the [[Mainfolder/Statistics/Standard error\|Standard Error]] of the mean
- **Shape**: As more dots are added, the bell shape emerges ([[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]])

### Example with Student Heights
Imagine measuring student heights:
- Each dot = mean height from a sample of 30 students
- 1000 different samples = 1000 dots
- Pattern shows typical values for sample means
- More dots near population mean, fewer at extremes

### Key Concepts
| Concept | Description |
|---------|-------------|
| Purpose | Shows variability of statistics across samples due to random chance |
| Practice | Usually work with one sample, but concept helps understand variability |
| Application | Used in [[inference\|inference]] and [[Mainfolder/Statistics/hypothesis testing\|hypothesis testing]] |

## Types of Distributions

| Type | Symbol | Description | Example |
|------|--------|-------------|----------|
| [[Mainfolder/Statistics/Population Distribution\|Population Distribution]] | $\mu$, $\sigma$ | Distribution of all values in population | All student heights |
| [[Sample Distribution\|Sample Distribution]] | $\bar{x}$, $s$ | Distribution of values in one sample | Heights of 30 students |
| [[Mainfolder/Statistics/sampling distribution\|Sampling Distribution]] | $\mu_{\bar{x}}$, $SE$ | Distribution of statistics from many samples | Means of many samples |

## Construction Process
| Step | Action | Notes |
|------|--------|-------|
| 1. Population | Start with population | Often unknown in practice |
| 2. Sampling | Take sample of size $n$ | Must be random |
| 3. Calculate | Compute desired statistic | Mean, proportion, etc. |
| 4. Repeat | Many times with same $n$ | Typically 1000+ times |
| 5. Plot | Create distribution of statistics | Usually approximately normal |

## Properties

### Center and Shape
| Property | Description | Mathematical Form |
|----------|-------------|-------------------|
| Center | Equal to population parameter | $E(\bar{x}) = \mu$ |
| Shape | Approaches normal distribution | Via [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] |
| Bias | Unbiased if center = parameter | $\text{Bias} = E(\text{statistic}) - \text{parameter}$ |

### Variability Measures
| Measure | Symbol | Formula | Description |
|---------|--------|---------|-------------|
| Population SD | $\sigma$ | - | Measures population variability |
| Sample SD | $s$ | $\sqrt{\frac{\sum(x-\bar{x})^2}{n-1}}$ | Estimates population variability |
| [[Mainfolder/Statistics/Standard error\|Standard Error]] | $SE$ | $\frac{\sigma}{\sqrt{n}}$ | Measures sampling variability |

## [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] (CLT)
### Key Points
| Aspect | Description |
|--------|-------------|
| Distribution Shape | Approaches normal as $n$ increases |
| Requirements | Independent random samples |
| Sample Size | Usually $n \geq 30$ is sufficient |
| Application | Works regardless of population shape |

### Effect of Sample Size
| Change in $n$ | Effect on Sampling Distribution |
|--------------|----------------------------|
| Increases | More normal shape |
| Increases | Smaller $SE$ ($\propto \frac{1}{\sqrt{n}}$) |
| Increases | Better estimate of parameter |

## Example: Movie Budgets (2012-2018)

### Population Parameters
| Parameter | Value |
|-----------|--------|
| Population Size | 1,056 movies |
| Population Mean ($\mu$) | $51.38 million |
| Time Period | 2012-2018 |

### Sampling Distribution Characteristics
| Sample Size | Characteristics |
|-------------|----------------|
| $n = 10$ | High variability, less normal |
| $n = 1000$ | Low variability, more normal |

### Mathematical Relationship
For means:
$$SE_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

For proportions:
$$SE_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$$

These concepts are fundamental for:
- [[Mainfolder/Statistics/Confidence Interval\|Confidence Interval]]
- [[Mainfolder/Statistics/hypothesis testing\|Hypothesis Testing]]
- [[Statistical Inference\|Statistical Inference]]
