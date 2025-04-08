---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/sampling distribution/"}
---

## Definition and Purpose
> A sampling distribution is the **distribution of statistics from many samples** (all with the same sample size)


- Shows **how much a statistic varies from sample to sample due to random chance**
- It's a theoretical tool; in practice, we usually only take one sample
- Purpose: Understand variability in estimates (statistics) from multiple samples

## Relationship to Other Distributions

| Distribution Type           | What It Represents                                                            |
| --------------------------- | ----------------------------------------------------------------------------- |
| [[Mainfolder/Statistics/Population Distribution\|Population Distribution]] | Distribution of a variable for the entire population (usually unknown)        |
| Sample Distribution         | Distribution of a variable for a single sample (used to calculate statistics) |
| Sampling Distribution       | Distribution of statistics from many samples of the same size                 |

## Constructing a Sampling Distribution
1. Start with the population
2. Take a sample and compute the statistic
3. Repeat steps 2-3 for multiple samples
4. Plot all statistics in a histogram or dot plot

## Properties of Sampling Distributions
- **Center**: Mean of the sampling distribution is close to the true parameter value
- **Shape**: Becomes more bell-shaped with larger sample sizes
- **Spread**: Decreases with larger sample sizes, improving precision

## [[Mainfolder/Statistics/Central Limit Theorem\|Central Limit Theorem]] (CLT)
- The sampling distribution of the mean approaches a normal distribution as sample size increases
- This occurs regardless of the shape of the population distribution
- Explains why the Normal distribution appears so often in statistics

## Variability in Sampling Distributions
- **Population Variability**: Described by population standard deviation (σ)
- **Sample Variability**: Described by sample standard deviation (s)
- **Sampling Variability**: Described by the standard error (SE)

## [[Mainfolder/Statistics/Standard error\|Standard Error]]
- Measures the variability of a statistic across different samples
- For means: SE = σ/√n (where σ is population standard deviation)
- Decreases as sample size increases (proportional to 1/√n)

## Effect of Sample Size
As sample size increases:
- The sampling distribution becomes more bell-shaped
- The standard error (SE) decreases, making estimates more precise

## Example – Movie Budgets
From the knowledge base:
- Data from Hollywood movies (2012-2018) with budgets in millions of dollars (n=1056)
- Population Mean (μ): 51.38 million dollars
- Sampling distribution with n=10 shows much more variability than with n=1000
