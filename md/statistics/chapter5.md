# Chapter 5: Discrete Probability Distributions

# Probability Distributions

### Terms

**Variable:** Characteristic that can assume different values

- **Discrete Variables:** Values are discrete quantitative units
    
    Example: Number of wheels
    
- **Continuous Variables:** Values are a point within a continuous range
    
    Example: Speed
    

**Random Variable:** Variable whose value is determined randomly

### Discrete Probability Distribution

**Discrete probability distribution:**

- Lists the discrete values a random variable can assume, and their corresponding probability
- Specific outcomes are notated as $X$; the probability of $X$ occurring is notated as $P(X)$
- Can be determined theoretically or empirically
    - Theoretically:
        - Where there are $n$ potential discrete values, and each has an equally random chance, the probability for each discrete value is $\frac {1} {n}$
            - Example: Discrete Probability Distribution for rolling a standard die
            
            | $X$ | 1 | 2 | 3 | 4 | 5 | 6 |
            | --- | --- | --- | --- | --- | --- | --- |
            | $P(X)$ | $\frac {1} {6}$ | $\frac {1} {6}$ | $\frac {1} {6}$ | $\frac {1} {6}$ | $\frac {1} {6}$ | $\frac {1} {6}$ |
        - For a compound event, which includes any of $r$ number of potential values, the probability for the compound event is $\frac {r} {n}$
            - Example: Discrete Probability Distribution for rolling an odd or even
            
            | $X$ | Odd | Even |
            | --- | --- | --- |
            | $P(X)$ | $\frac {1} {2}$ | $\frac {1} {2}$ |
    - Empirically:
        - Determined by observing the outcome of numerous trials. For $n$ trials, the probability for each value that occurred $r$ times is $\frac {r} {n}$

### Discrete Probability Distribution Requirements

The sum of all probabilities within a sample space must be 1.

$$
\Sigma P(X)=1
$$

The probability of each event cannot be lower than 0 or greater than 1.

$$
0 \le P(X) \le 1
$$

# Mean, Variance, Standard Deviation, Expectation

### Mean

**Mean:**

To calculate the mean for discrete quantitative data, sum the products of each value with its frequency.

$$
\mu = \Sigma X \cdot P(X)
$$

### Variance, Standard Deviation

**Variance:**

To calculate the variance for discrete quantitative data, sum the products of the square of the difference between each value and the mean with the value’s frequency.

$$
\sigma ^2 = \Sigma \big( ( X - \mu ) ^2 \cdot P(X) \big)  
$$

**Variance shortcut formula:**

There is a shortcut formula for calculating the variance:

$$
\sigma ^2 = \Sigma \big( X ^2 \cdot P(X) \big) - \mu ^2
$$

**Standard deviation:**

The standard deviation is the square root of the variance; $\sqrt{\sigma^2}$, or:

$$
\sqrt{\Sigma \big( X ^2 \cdot P(X) \big) - \mu ^2}
$$

### Expectation

**Expectation:** The expected return from a trial

- Similar formula as mean, however, instead of using the raw output value, it adjusts the output for an expense incurred at input
    - Example: If a lottery ticket costs 1 and has a chance of winning 1000, the mean would calculate the potential results as 0 and 1000; the expectation would adjust for the input cost, and calculate the potential results as -1 and 999.

# Binomial Distribution

### Binomial Distribution

**Binomial Distribution:**

- Takes a trial repeated identically $n$ times; each trial has two potential outcomes - success or failure; the rate of success for an individual trial is known; calculates the probability that over $n$ trials there will be $X$ successes.

### **Formula**

Formula for calculating a binomial distribution:

where 

- $n$ is the number of trials;
- $p$ is the probability of success;
- $q$ is the probability of failure ($q=1-p$); and
- $X$ is the amount of successes;

the probability that in $n$ trials specifically $X$ trials will be successful is calculated as follows:

$$
P(X) = \space _n C _x \cdot p ^X \cdot q ^{n-X}
$$

### Binomial Distribution Table

**Binomial Distribution Table:**

- There is a precalculated table which lists the probabilities of binomial distributions.
- The table takes $n$, $X$, and $P(S)$, and lists $P(X)$

### Mean, Variance, Standard Deviation for Binomial Distribution

Binomial Distributions have specific shortcut formulas for calculating their statistical measures:

- Mean

$$
\mu = n \cdot p
$$

- Variance

$$
\sigma ^2 = n \cdot p \cdot q
$$

- Standard Deviation

$$
\sigma = \sqrt {n \cdot p \cdot q}
$$
