# Chapter 3: Data Description

# Measures of Central Tendency

### Parameters vs Statistics

**Parameters:** taken from the entire population

**Statistics**: taken from a sample

### Mean

**Mean:** Arithmetic average

**Notations:**

- $\mu$ for population
- $\overline{X}$ for sample

**Formula:**

$$
\mu =\frac {\Sigma X} {n}
$$

where

- $X$ is the data; and
- $n$ is the number of values

### Mean for Weighted Data

**Calculation:**

- To find $\Sigma X$, sum the product of each value and its corresponding weight
- To find $n$, sum the weights

**Formula:**

$$
\frac {\Sigma (X \cdot w)} {\Sigma w}
$$

where

- $X$ is the data; and
- $w$ are the weights

### Mean for Grouped Data

**Calculation:** To find $\Sigma X$, sum the midpoints of each class, weighted by the class frequency

**Formula:**

$$
\frac {\Sigma (f \cdot X_m)} {n}
$$

where

- $f$ is the class frequency;
- $X_m$ is the class midpoint; and
- $n$ is the number of values

### Median

**Median** **(MD)**: Value in the middle of the data set.

- Where n is odd, the middle value
- Where n is even, the average of the two middle values

### **Median of grouped data**

1. Find the group with the median value
2. Find the ratio of how many values into the group the median is ($\frac {value \space index}{class \space frequency}$)
3. Apply the ratio to the class width; add to class lower boundary
    
Example:
    
- $n$: 61
- Class with $i_{31}$ contains the median
- Class “15-20” contains $i_{30}-i_{36}$
- $i_{31}$ is 2 values into the class
- The class frequency is 7
- The ratio of the values into the class the median is is $\frac {2} {7}$
- The class width is 5
- The applied ratio is $\frac {10}{7}$
- The lower boundary is 14.5
- With the added $\frac{10}{7}$ we round to 16
- Median is: 16

### Mode

**Mode:** most often occurring value

- Data can be **unimodal, bimodal,** **multimodal,** or have no mode.
- For grouped data, the class with the highest frequency is the **modal class.**

### Midrange

**Midrange** **(MR):** average of min and max

### Outliers

**Outliers:** Extremely high or low values

### Distribution Shapes

- **Symmetric distribution**:
    
    [](https://lh7-us.googleusercontent.com/kc-CBwL5DrWQlv0eh-n1fupBdhaF89R1Adl_hhHsh5ErIrMXlisf2RlTufvQg4K3Ot1oWl8X7VyLob60ERN2RBpI-X5u73LD0QHDvPqJx9Zz9iXM4mn0KuzEHIa6QC1_BUCDGSeMwdZRzI9sW4S2xoQ)
    
    - Data is evenly distributed on both sides of the mean
- **Right skewed** /**positively skewed**:
    
    [](https://lh7-us.googleusercontent.com/kosST66RBq3i6vzrm-FgoGdwnYgq87d6nNs2H0en-oZrrD_8o-t3UDNBOyzJvLXcHH9yCZ0o229NofAuEMGIWxDWvJdabPa7-WMpXFHQsGfwLS83bp4xh4CjvqFCtD3GU2JphSCP9gtFcQnnvD11Ldo)
    
    - Most of the data is on the left side of the mean; the mean is pulled right due to right outliers
    - The median is to the left of the mean
    - Generally, the mode is to the left of the mean and the median
- **Left skewed** / **negatively skewed**:
    
    [](https://lh7-us.googleusercontent.com/rod5Su3kXTPHiwJaAtf9MxcZtfdcy_K5fgx88OrkMIbyN47ewRpsUKz4lu3YduS0Nds-DhEoEOY3QwabqTA8CW6bCK_fdkzyLtALCH7SoSW3hR2OshvAWm4EMfSoeMcv1x5iTGjyLraKv9WrPPO9--k)
    
    - Most of the data is on the right side of the mean; the mean is pulled left due to left outliers
    - The median is to the right of the mean
    - Generally, the mode is to the right of the mean and the median

---

# Measures of Variation

### Range

**Range (R)**: Distance between the highest and lowest values

**Formula:**

$$
X_{max}-X_{min}
$$

### Variance, Standard Deviation

**Deviation:** A value’s deviation is its distance from the mean

**Population Variance** $(\sigma ^2)$**:**

- Average squared data point deviation for the population data
- Measures the distribution spread
- Formula:

$$
{ \frac{\Sigma(X-\mu)^2}{n} }
$$
    
where:
    
- $X$ is the individual data;
- $\mu$ is the population mean; and
- $n$ is the number of values

**Population Standard Deviation** $(\sigma)$**:**

- Quadratic mean of the deviation of population data
- Square root of the population variance
- Formula:

$$
\sqrt { \frac{\Sigma(X-\mu)^2}{n} }
$$

**Sampled Data Standard Deviation** $(s)$ **and Variance** $(s^2)$**:**

- $(n - 1)$ is used in the denominator instead of $n$
- Formula:
    
$$
\sqrt { \frac{\Sigma(X-\overline{X})^2}{n-1} }
$$
    
where:
    
- $X$ is the individual data;
- $\overline{X}$ is the population mean; and
- $n$ is the number of values
    
There is a shortcut formula which does not require a precalculated mean:
    
$$
\sqrt{ \frac{n(\Sigma X^2)-(\Sigma X)^2}{n(n-1)} }
$$
    
**Grouped Data Standard Deviation:** Class midpoint’s deviation, weighted by class frequency

Shortcut formula:

$$
\sqrt{ \frac{n(\Sigma f \cdot X_{m}^2)-(\Sigma f \cdot X_m)^2}{n(n-1)} }
$$

### Coefficient of Variation

**Coefficient of Variation:** Standard for variance measurement; ratio of standard deviation to mean

- For populations: $(\frac{\sigma}{\mu}\cdot 100) \%$
- For samples: $(\frac{s}{\overline{X}}\cdot 100) \%$

### Distribution Rules

**Range rule of thumb:** The standard deviation is roughly a quarter of the range

Formula:

$$
s \approx \frac {range}{4}
$$

**Chebyshev’s Theorem:** finds percentage of values within $x$ standard deviations from the mean; applicable to all distribution shapes:

Theorem: Within $k$ standard deviations from the mean will be at least $(1- \frac{1}{k^2})\%$ of the values, where $k$ is greater than 1.

- $75\%<2\sigma$
- $88.9\%<3\sigma$

**Empirical** **Rule:** finds percentage of values within $x$ standard deviations from the mean in a **normal** / **bell-shaped** distribution:

- $68\%<1\sigma$
- $95\%<2\sigma$
- $99.7\%<3\sigma$

---

# Measures of Position

### Z Score

**Z score:** Value’s standard-deviation units from the mean

**Calculation:** Distance from the mean divided by the standard deviation

Formula:

$$
\frac{X-\overline{X}}{S};\frac{X-\mu}{\sigma}
$$

### Percentiles

**Percentiles** divide data into 100 groups

1% of data is below $P_1$, 20% below $P_{20}$ etc.

**Calculation:** To find the percentile of $X$ within a dataset with $n$ values, divide $X$’s cumulative frequency by $n$

Formula:

$$
(\frac{X_{CF}}{n}\cdot100)\%
$$

**Tweaked Formula:** To obtain a more representative view, we use a tweaked formula:

- **To find the percentile of a value:**

Calculation: The number of values less than $X$ plus 0.5, over $n$
    
Formula:
    
$$
(\frac{n_{<x}+0.5}{n}\cdot 100)\%
$$

- **To find the value corresponding to a percentile:**
  - First, find $\frac{n\cdot P}{100}$
  - If $\frac{n\cdot P}{100}$ is a fraction, round up and find the correspondingly ranked data

  - Formula:

$$
X_{\lceil \frac{n\cdot P}{100} \rceil}
$$
        
  - If $\frac{n\cdot P}{100}$ is a whole number, use the average of the value with that rank and the next value

  - Formula:
        
$$
\text{average}({X_{ \frac{n \cdot P}{100} }, \space X_{ \frac{n \cdot P}{100} +1}})
$$
        

### Quartiles

**Quartiles** divide data into 4 groups:

- $Q_1=P_{25}$
- $Q_2=P_{50}$
- $Q_3=P_{75}$

**For a more direct quartile formula:**

- $Q_2$: Median of all values
- $Q_1$: Median of values below $Q_2$
- $Q_3$: Median of values above $Q_2$

### Interquartile Range

**Interquartile range (IQR):** $Q3-Q1$

**Procedure to identify outliers:** $Q1-(IRQ \cdot 1.5)$ or $Q3+(IRQ \cdot 1.5)$

### Decile

**Decile** divides data into 10 groups; $D_1=P_{10}$…

---

# **Exploratory Data Analysis**

**Five number summary:** Includes

- Min
- Q1
- Median
- Q3
- Max

**Boxplot:** Graph of five number summary: Vertical line at median; box extending to Q1 and Q3; horizontal line in middle of box to min and max.

Example:

[](https://lh7-us.googleusercontent.com/Yy0zVKY4vuJ3h2pwcHjzz6FxYFAqwK8pocjBPYK2qz7V9crUM7QRL6VvBkkHxaLPLaocsmNTULznnB--l1h-njG16TozHAIxvDPfmalaxhcZwy8Cy79xjjLT50piNHhR6GSudY_x6UsFZ0V8ueZzzZY)

- $\min=3$
- $Q_1=9$
- $\text{med}=18$
- $Q_3=21$
- $\max = 27$
