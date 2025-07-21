---
{"dg-publish":true,"permalink":"/Academic/Statistics/Numerical Summaries/"}
---

>**Numerical Summaries** calculating numbers that tell us about certain aspects of the data

Here are some key concepts:
1. [[Academic/Statistics/Center\|Center]]
2. [[Academic/Statistics/Spread\|Spread]]
3. [[Academic/Statistics/Shape\|Shape]]
4. [[Academic/Statistics/Outliers\|Outliers]]

Basically, when we wish to discuss about **center** and **spread**, there are two separate approach:

- [[Academic/Statistics/Order Statistics\|Order Statistics]]
- [[Academic/Statistics/moment statistics\|moment statistics]]

---
***Which statistics we should use?*** 

The ***shape of the distribution***, as well as whether we have outliers will determine whether we use order statistics (median and IQR) or moment statistics (mean and standard deviation) to describe the center and spread

In general we prefer to use moment statistics (mean and standard deviation) if we can, but there are certain situations where the mean and standard deviation are not good measures of center and spread

Here are some situations:
- A **skewed distribution** can affect the mean and std. dev. a lot ---> Median and IQR
- **Outliers** can affect the mean and std. dev. a lot ---> Median and IQR

**Symmetric shape with no ’extreme’ outliers → mean and std. dev.
Skewed shape or outliers (or both) → median and IQR**


---
## Parameters and statistics
**Statistics** are numerical summaries calculated from the sample. 
- typically statistics are denoted using lowercase English alphabet characters 
	-  sample mean = $x$ 
	-  sample standard deviation = $s$

**Parameters** are numerical summaries calculated from the population. 
- typically parameters are denoted using Greek alphabet characters 
	-  population mean = $\mu$ 
	-  population standard deviation = $\sigma$ 
- almost always the value of parameters are **unknown** to us (we want to learn about their values)

---
## Z-scores

**Standardizing our value**s is a way of adjusting them so that we can directly compare them. These adjusted values are called [[Academic/Statistics/z-scores\|z-scores]].

*It is important because it can help us compare two variables that measure similar things but use different scales.*

