# Chapter 8: Hypothesis Testing

# Overview

### Scientific Hypotheses and Errors

**Hypothesis:**

- In the scientific method, a claim is represented as two opposing hypotheses:
- **Alternative Hypothesis;** $H_1$**:**
    - The alternative hypothesis, or H1, makes an active claim.
- **Null Hypothesis;** $H_0$**:**
    - The null hypothesis, or H0, is passive.
- The null hypothesis is assumed until there is sufficient evidence to reject it and accept the alternative hypothesis.

Error types:

- **Type I Error:**
    - The null hypothesis is true but is rejected.
- **Type II Error:**
    - The null hypothesis is false but is not rejected.

### Inferential Statistics

**Inferential Statistics:**

- Infers population parameters from sample statistics

**Statistical Hypothesis:**

- Hypothesis about population parameters based on sample statistics

### Scientific Method for Inferential Statistics

The procedure for scientifically processing statistical hypotheses is as follows:

- Hypothesis:
    - H0:
        - The null hypothesis assumes that the sample mean is congruent with a given population mean, and no new parameters can be inferred from the statistics.
    - H1:
        - The alternative hypothesis actively claims that the sample mean is incongruent with the given population mean, and new parameters can be inferred from the statistics.
- Testing:
    - A threshold of acceptable sample mean improbability is assumed.
    - The central limit theorem is used to test the probability of the sample mean given the given population mean.
    - If the sample mean lies within the accepted threshold, the null hypothesis is not rejected, and there is insufficient evidence to accept the alternative hypothesis.
    - If the sample mean lies beyond the accepted threshold, the null hypothesis is rejected, and there is sufficient evidence to accept the alternative hypothesis.

### Catch A Test By Its Tail

There are three types of test tails, dependent on the given alternative hypothesis:

- **Right-tailed:**
    - In a right-tailed test, H1 claims that data is above a given mean.
    - Example:
        - The mean number of books read per year for the average adult is 20. A sample of 12 chiropractors has a mean of 23 books read per year. Can we conclude that chiropractors read more books on average than the average adult?
        - H0: $\mu = 20$
        - H1: $\mu>20$
- **Left-tailed:**
    - In a left-tailed test, H1 claims that data is below a given mean.
    - Example:
        - The given mean number of crashes per day is 85. A sample of 3 days, however, has a mean of 79. Can we conclude that the mean is in fact less than 85?
        - H0: $\mu = 85$
        - H1: $\mu < 85$
- **Two-tailed:**
    - In a two tailed test, H1 claims the data does not equal a given mean, and can deviate in either direction.
    - Example:
        - The mean heartrate for adults is 85. A sample of 1200 participants treated with a specific drug has a mean heartrate of 88. Can we conclude that the drug affects heartrates?
        - H0: $\mu=85$
        - H1: $\mu\not = 85$

### Valuable Terms

**Level of Significance;** $\alpha$**:**

- The level of significance is the accepted threshold of probability of a Type I error:
    - A Type I error is when H0 is incorrectly rejected
    - When data is used to reject H0, there is a possibility that H0 is actually correct, and the data is an outlier.
    - The probability of a Type I error is dependent on the probability of the sample mean given the given parameter.
        - Example:
            - The population mean is 20. The sample mean is 22. Is the sample mean sufficient to support a claim that $\mu>20$?
            - If there is a 0.11 probability of the sample mean being 22 for the given population mean, using the sample mean to reject H0 has a 0.11 chance of being a Type I error.

**P Value:**

- The P value is the statistic’s probability, assuming H0.
- If the P value is above $\alpha$, H0 is not rejected. If the P value is below $\alpha$, H0 is rejected, and there is sufficient evidence to support H1.

**Critical Value; CV:**

- The critical value, or CV, is the distribution point beyond which statistics have significance and are sufficient evidence to reject H0.

**Critical Region:**

- The critical region is the range of values within which statistics have significance and are sufficient evidence to reject H0.

# Z-Test

### Z Test

The **Z Test** is the traditional method for assessing statistical hypotheses.

- A critical value is established.
- If the test value is past the critical value threshold, H0 is rejected.

### Finding the Z Test Critical Value

The critical value is established by finding the $z$ score for the given $\alpha$.

- Right-Tailed Test:
    - The critical value is the $z$ score with an area of $\alpha$ to its right.
        - Example:
            - Question:
                - Find the critical value for a right-tailed test with $\alpha=0.05$.
            - Answer:
                - According to the normal distribution, $z=1.64$ has $0.05\%$ to its right.
- Left-Tailed Test:
    - The critical value is the $z$ score with an area of $\alpha$ to its left.
        - Example:
            - Question:
                - Find the critical value for a left-tailed test with $\alpha=0.01$.
            - Answer:
                - According to the normal distribution, $z=-2.33$ has $0.01\%$ to its left.
- Two-tailed Test:
    - Since the two-tailed test utilizes deviations in both directions, the total $\alpha$ is split between the right tail and the left tail.
    - The critical value is the absolute $z$ score that has beyond it on either side of the mean an area of $\alpha/2$.
        - Example:
            - Question:
                - Find the critical value for a two-tailed test with $\alpha=0.05$.
            - Answer:
                - Since this is a two tailed test, the critical value is $z_{\alpha/2}$.
                - According to the normal distribution, $z\pm1.96$ has beyond it on either side of the mean an area of $0.025$.

### Common Critical Values

|  | Left-Tailed | Right-Tailed | Two-Tailed |
| --- | --- | --- | --- |
| $\alpha=0.1$ | -1.28 | 1.28 | $\pm$1.64 |
| $\alpha=0.05$ | -1.64 | 1.64 | $\pm$1.96 |
| $\alpha=0.01$ | -2.33 | 2.33 | $\pm$2.58 |

### Using the Z Test

To use the Z test, the corresponding test statistic is calculated and compared to the critical value.

The formula for the sample $z$ score is:

$$
z = \frac{\bar{X} - \mu}{\sigma/\sqrt{n}}
$$

where:

- $\bar{X}$ is the sample mean; and
- $\mu$ is the hypothesized population mean; and
- $\sigma$ is the population standard deviation; and
- $n$ is the sample size.

### Example

- Question:
    - For a population mean of 26 and standard deviation of 3, can a $n=32$ sample with a mean of 24.5 be used to reject H0 in a left tailed test with $\alpha=0.1$?
- Answer:
    - For a left-tailed test with $\alpha=0.1$, $z=-1.28$.
    - Calculating the statistic $z$ score gives us:
        
        $$
        z=\frac{24.5-26}{3/\sqrt{32}}\approx-2.83
        $$
        
    - Since the test statistic $z=-2.83$ is past the $\alpha$’s $z=-1.28$, H0 is rejected, and there is sufficient evidence to support H1.

# P-Value Method

### P-Value Method

A similar method to the $z$ test is the $P$-value method.

- The $P$-value method calculates the statistic $P$-value, which is the probability of the statistic assuming H0.
- If the statistic $P$-value is greater than $\alpha$, H0 is not rejected.
- If the statistic $P$-value is equal or less than $\alpha$, H0 is rejected, and there is sufficient evidence to accept H1.

### Finding the P-Value

To find the statistic $P$-value, find the $z$ score, and the corresponding probability.

### Example

- Question:
    - For a population mean of 26 and a standard deviation of 3, can a $n=33$ sample with a mean of 26.1 be used to reject H0 in a right-tailed test with $\alpha=0.05$?
- Answer:
    - Calculating the statistic $z$ score gives us:
    
    $$
    z=\frac{26.1-26}{3/\sqrt{33}}\approx 0.19
    $$
    
    - According to the normal distribution, the area to the right of $z=0.19$ is 0.4247.
    - The $P$-value 0.4247 is more than $\alpha=0.05$.
    - Since the $P$-value is greater than $\alpha$, H0 is not rejected.

# Student T Distribution

### Instances of T Distribution Necessity

The $z$ test and $P$-value method both use the statistic $z$ score.

As noted in earlier chapters, the $z$ score cannot be used when the sample size is less than 30 and population standard deviation or distribution shape is unknown.

Instead, the T distribution is used.

Note: the T distribution requires that the sample data is approximately normally distributed.

### Calculating the T Distribution Critical Value

To calculate the critical value using the T Distribution, find the $t$ value for the given degrees of freedom and $\alpha$.

<aside>
<img src="https://www.notion.so/icons/arrow-right-basic_gray.svg" alt="https://www.notion.so/icons/arrow-right-basic_gray.svg" width="40px" /> Reminder: $d.f.=n-1$

</aside>

- Right-tailed test:
    - For a right-tailed test, find the $t$ value with an area of $\alpha$ to its right.
- Left-tailed test:
    - For a left-tailed test, find the $t$ value with an area of $\alpha$ to its left.
- Two-tailed test:
    - For a two-tailed test, find the absolute $t$ value that, on both sides of the mean, has beyond it an area of $\alpha/2$.

### Using the T Distribution Critical Value

To use the T Test critical value, calculate the corresponding $t$ value for the given $\alpha$, sample degrees of freedom, which is $n-1$, and tail type.

Next, find the statistic $t$ value, using the sample standard deviation:

$$
t = \frac{\bar{X}-\mu}{s-\sqrt{n}}
$$

Compare the statistic $t$ value with the critical value; if the $t$ value is beyond the critical value, reject H0.

### T Distribution Critical Value Example

- Question:
    - For a population mean of 19, can a $n=12$ sample with a mean of 20.3 and standard deviation of 1.4 be used to reject H0 in a right-tailed test with $\alpha=0.01$?
- Solution:
    - For $\alpha=0.01$ and $d.f.=11$, the right-tailed $t$ value is 2.72.
    - Calculating the statistic $t$ value gives us:
        
        $$
        t = \frac{20.3-19}{1.4/\sqrt{12}}\approx 3.22
        $$
        
    - Since the statistic $t$ value is beyond the critical value, H0 is rejected.

### Calculating the T Distribution P Value

Finding the $P$-value for a T distribution is difficult, as T distribution tables provide the $t$ values for discrete areas at large intervals, and finding the precise area for a given $t$ value is difficult.

Instead, a range of $P$-values is used, corresponding to the two areas between which the $t$ score lies.

Example:

- Question:
    - Find the $P$-value for a single-tailed test where $t=1.42$ and $d.f.=16$.
- Answer:
    - For $d.f.=16$, $t=1.42$ lies between 1.337 and 1.512, which have areas of 0.1 and 0.075.
    - The $P$-value interval is: $0.075<P<0.1$.

### Using the T Distribution P Value

When using the T Distribution $P$-value, H0 can only be rejected if the entire range for the $P$-value is lower than $\alpha$.

Example:

- For $.15<P<.2$ and $\alpha=.25$, reject H0.
- For $.001<P<.005$ and $\alpha=.0025$, do not reject H0.

### T Distribution P Value Example

- Question:
    - For a population mean of 19, can a $n=12$ sample with a mean of 20.3 and standard deviation of 1.4 be used to reject H0 in a right-tailed test with $\alpha=0.01$?
- Solution:
    - Calculating the statistic $t$ value gives us:
        
        $$
        t = \frac{20.3-19}{1.4/\sqrt{12}}\approx 3.22
        $$
        
    - For $d.f.=11$, $t=3.22$ lies between 3.106 and 4.025, which have areas of .005 and .001.
    - The $P$-value interval is $.001<P<.005$
    - $\alpha=.01$ is greater than the entire $.001<P<.005$ range.
    - Since the $P$-value is lower than $\alpha$, H0 is rejected.