# Chapter 7: Confidence Intervals and Sample Size

# Point Estimate, Interval Estimate

### Parameters, Statistics

**Statistic:**

- Data about a sample

**Parameter**:

- Data about a population

Statisticians often aim to estimate parameters based on statistics.

### Point Estimate

**Point Estimate**:

- A point estimate is a specific point for the parameter inferred from statistics.
- The best point estimate for the population $\mu$ is $\bar{X}$.
- However, point estimates are generally imprecise, due to sampling error.

### Interval Estimate

**Interval Estimate:**

- An interval estimate gives a range of values for the parameter, instead of a single point.
- An interval estimate can be linked with a level of confidence - there is an $x$ probability that, based on the sample mean, the population mean is between $a$ and $b$.
    - A **confidence interval** is an interval estimate with a given **confidence level**.
    - A confidence interval is often given as a **margin of error** from the mean, which is the margin the interval estimate deviates on either side of the mean.
        - Example:
            
            $$
            65 \pm 1.4
            $$
            
            represents a mean of 65 and margin of error of 1.4.
            
            The total represented confidence interval is:
            
            $$
            63.6<\mu<66.4
            $$
            

# Confidence Interval Formula Explanation

### Confidence Interval Formula Explanation

1. In the last chapter, we used the central limit theorem and normal distribution to find the value of a sample mean relative to the population mean.
    
    Here, we do the opposite: we find the population mean relative to the sample mean.
    
2. If we know the population standard deviation and the sample size, we can calculate the $z$ value for a given distance between $\mu$ and $\bar{X}$:

$$
z = \frac {\bar{X} - \mu} {\sigma / \sqrt{n}}
$$

1. If $p\%$ of values are within $z=s$, then there is a $p\%$ chance that, for a given value, the mean is within $z=s$.
2. In the normal distribution, 90% of values are within 1.645 standard deviations of the mean - 45% within 1.645 to the right, and 45% within 1.645 to the left.
    
    By extension, there is a 90% probability that, for a given sample mean, the population mean is within $z=1.645$ deviations. Thus, we can estimate the population mean within a 90% confidence level.
    
    We can use this method to find the confidence range for any confidence level, by replacing $z=1.645$ with the $z$ corresponding to the given confidence level.
    
3. The notation for the $z$ value of a given confidence level is:
    
    $$
    z_{\alpha/2}
    $$
    
    where $alpha$ refers to the total area of the tails which are not included in the confidence interval.
    
    The $alpha$ is calculated as 1 minus the given probability.
    
    For a 90% confidence level, which calculates a .9 probability, the total tail area is .1.
    
    As the total tail area is .1, the area for the tail of each side is .05.
    
    The corresponding $z$ value is that which, when deviated on one side of the mean, has, on that side, a tail of .05 - $\alpha/2$ - and includes .45.
    
4. Once the $z$ value is found, it can be implemented for the specific sample to find the **margin of error**, or $E$. The margin of error is the interval in which the parameter may be, for the given confidence level, above or below the sample mean.
    
    The formula for the confidence interval, for a given mean and margin of error, is:
    
    $$
    \bar{X}-E<\mu<\bar{X}+E
    $$
    
    The formula for finding the margin of error, or $E$, for a given sample, is:
    
    $$
    E = z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})
    $$
    
    Substituting this for $E$ in the previous formula give us the final confidence interval formula:
    
     
    
    $$
    \bar{X}-z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})<\mu<\bar{X}+z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})
    $$
    

# Using the Confidence Interval Formula

### Confidence Interval Formula

The confidence interval formula calculates the confidence interval of the population mean from a given sample mean.

### Requirements

Requirements for using the confidence interval formula:

- The population must be normally distributed, or the sample must be $n ≥ 30$.
- The population standard deviation must be known, or, if it is unknown and $n≥30$, the sample standard deviation can be used instead.
- If these requirements are not met, the $t$ distribution - explained below - is used instead.

### Formula

The formula for the confidence interval is:

$$
\bar{X}-z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})<\mu<\bar{X}+z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})
$$

### Common $Z$ Values

There are three commonly used confidence levels: 90%, 95% and 99%.

Their corresponding $z_{\alpha/2}$ values are:

| **confidence interval** | **z** |
| --- | --- |
| 90 | 1.645 |
| 95 | 1.96 |
| 99 | 2.576 |

### Example

Question:

- For a sample where $n=45$, the sample mean is 85 and the standard deviation is 6.1, what is the 99% confidence interval for the population mean?

Solution:

- The $z$ value for a 99% confidence interval is: 2.576.
- Substituting the given values in the margin of error formula gives:
    
    $$
    E = 2.576(\frac{6.1}{\sqrt{45}}) \approx 2.3
    $$
    
- The final confidence interval is:
    
    $$
    85 \pm 2.3
    $$
    

# Finding the Sample Size

### Sample Size Formula

The confidence interval formula can be rearranged to find the ideal sample size for a given standard deviation, margin of error and confidence level.

The formula for the margin of error is:

$$
E = z_{\alpha/2}(\frac {\sigma} {\sqrt{n}})
$$

which can be rearranged to:

$$
n=( \frac {z_{\alpha/2} \cdot \sigma} {E} ) ^2
$$

The answer is then rounded up to the next whole number.

### Example

Question:

- For a population with a standard deviation of 8, how large must the sample size be to calculate the population mean within a margin of error of 3.5 at a 95% confidence level?

Solution:

- The $z$ value for a confidence interval of 95% is: 1.96.
- Substituting the given values in the formula gives:
    
    $$
    n = \big(\frac {1.96 \cdot 8} {3.5} \big) ^2 =20.0704
    $$
    
    which is rounded up to 21.
    

# Student T Distribution

### Student T Distribution

Where the normal distribution confidence interval formula cannot be used, due to the sample size being less than 30, and the population standard deviation or population distribution shape being unknown, the **Student T Distribution** is used instead.

The T Distribution provides a larger margin of error than the standard distribution, due to additional uncertainty due to the variance or sample shape being unknown, and the small sample size.

The T Distribution requires that the sample data is approximately normally distributed.

### T Distribution Confidence Interval Formula

The T Distribution confidence interval formula is similar to the normal distribution formula, however, it uses a $t$ value instead of a $z$ value, and the sample standard deviation is used instead of the population standard deviation:

$$
E = t_{\alpha/2}(\frac {s} {\sqrt{n}})
$$

The confidence interval formula, then, is:

$$
\bar{X}-t_{\alpha/2}(\frac {s} {\sqrt{n}})<\mu<\bar{X}+t_{\alpha/2}(\frac {s} {\sqrt{n}})
$$

### Finding the $T$ Value

The $t$ value is found by consulting a distribution table.

The table takes the confidence level and the **degrees of freedom**.

- The degrees of freedom is one less than the sample size: $n-1$.

### Example

Question:

- For a sample where $n=15$, the sample mean is 85 and the standard deviation is 6.1, what is the 99% confidence interval for the population mean?

Answer:

- First, we find the corresponding $t$ value. For a sample size of $n=15$, the degrees of freedom is 14.
- Consulting the $t$ distribution table returns a $t$ value of 2.977 for $d.f.=14$ and $c=.99$.
- Substituting the given values in the formula for the margin of error gives:
    
    $$
    E = 2.977(\frac{6.1}{\sqrt{15}}) \approx 4.7
    $$
    
- The final confidence interval is:
    
    $$
    85 \pm 4.7
    $$