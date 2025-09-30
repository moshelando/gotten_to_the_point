# Chapter 4: Probability and Counting Rules

# Sample Space and Probability

## General Terms

**Probability Experiment:** Random process with well defined potential results

**Outcome:** Result of a probability experiment

**Event:** Set of one or more outcomes

- **Simple event:** Event which includes a single outcome, such as rolling a four
- **Compound event:** Event which can be any of multiple outcomes, such as rolling odd

**Tree diagram:** Branched diagram showing all possible outcomes of a probability experiment

**Sample Space:** Set of all possible results of a probability experiment

## Classical Probability

**Classical Probability:** Deals with events with equally likely sample space outcomes

Formula:

$$
P(E)=\frac{n(E)}{n(S)}
$$

where:

$P(E)$ is the probability of event $E$ occuring;

$n(E)$ is the number of outcomes included in event $E$; and

$n(S)$ is the total number of outcomes

**Probability Rules:**

Events have a chance between 0 and 1 to occur

0 is impossible. 1 is definite.

The total of all sample space events is 1

**Complementary Events:**

An event’s complementary event is an event’s negation; all outcomes *not* included in the event

Notation: 

Event: $E$

Event complementary: $\overline{E}$

Formula:

$$
E+\overline{E}=1
$$

## Empirical Probability

**Empirical Probability:** Deals with outcomes which do not have an equal chance of occurring, rather, each outcome has a relative frequency

The frequency table is constructed based on experiments

Formula:

$$
P(E)=\frac{f(E)}{n}
$$

where:

$P(E)$ is the probability of event $E$ occurring;

$f(E)$ is $E$’s relative frequency; and

$n$ is the sum of all frequencies

## Subjective Probability

**Subjective Probability** uses a probability value based on an educated guess

# **The Addition Rules for Probability**

## Addition Rules

**Addition Rules:** Calculate the probability that *either* of multiple events will occur; “A *or* B”

- **Mutually Exclusive Events:** Events that have no shared outcomes
    
    Where two events are mutually exclusive, the probability for “A or B” to occur is the probability for A plus the probability for B
    
    Formula:
    
    $$
    ⁍
    $$
    
- **Non mutually exclusive events:**
    
    Where two events are non mutually exclusive, the probability for “A or B” to occur is the probability for A, plus the probability for B, *minus* the probability of “A and B” occurring
    
    Reasoning: events which overlap A and B were counted twice
    
    Formula:
    
    $$
    P(AB)=P(A)+P(B)-P(AB)
    $$
    

# **The Multiplication Rules and Conditional Probability**

## **Multiplication Rules:**

**Multiplication Rules:** Calculates the probability that *all* of multiple results will occur; “A *and* B”

**Independent Events:** Separate events in which one does not affect the outcome of the other

The probability of two independent events both occurring is the product of both events’ probability

Formula:

$$
P(AB)=P(A)\cdot P(B)
$$

**Dependent Event:** Events in which the outcome of one is affected by and dependent on the outcome of the other

**Conditional Probability:** Where event A affects the probability of event B, the probability of event B happening after event A happens is expressed as:

$$
P(B|A)
$$

**Dependent events multiplication rules:** The probability of two dependent events both occurring is the product of the both events’ probability:

Formula:

$$
P(AB)=P(A) \cdot P(B|A)
$$

**Conditional Probability Rule:** To specifically find the probability of event B occurring assuming event A has already occurred, divide P(AB) by P(A), since we’re assuming A already occurred, and are not accounting for A’s probability.

Formula:

$$
P(B|A) = \frac{P(AB)}{P(A)}
$$

# **Counting Rules**

## **Fundamental Counting Rule**

**Fundamental Counting Rule:** When multiple independent events have numerous possibilities, the number of total possibilities is the product of all the events’ possibilities

Example:

Event A has three possibilities, Event B has five, Event C has two.

$n_1 = 3;\space n_2=5; \space n_3=2$

$n_1\cdot n_2\cdot n_3= 30$

## Permutation

**Permutation:** Specific sequence of a set number of items

**Notation:** The permutations of $n$ objects is expressed as $_nP$

**Rule:** $n$ objects have $n!$ total permutations

Formula:

$$
_nP=n!
$$

**Where the sequence will only have** $r$ **elements, and not all** $n$ **elements:** The permutations are expressed as $_nP_r$

To calculate: Divide the number of total $n$ permutations by the permutations of the difference between $r$ and $n$

Reasoning: each permutation with only $r$ elements is repeated again for each permutation of the subsequent elements

Formula:

$$
_nP_r=\frac{n!}{(n-r)!}
$$

**Where there is $r$ number identical items:** Divide $n!$ by $r!$

Reasoning: The specific sequence of the $r$ elements do not matter; the permutations were repeated for each individual $r!$ permutation.

Formula:

$$
\frac{n!}{r!}
$$

Example: If there are 12 total items, and 3 of them are identical, the total permutations is $\frac{12!}{3!}$

**If there are multiple repeated values:** Divide $n!$ by the product of the $r!$s

Reasoning: The total number of repeats is the product all the $r!$s; each individual $r!$ was repeated for each permutation of the other $r!$s

Formula:

$$
_nP=\frac{n!}{r_1! \cdot r_2! \cdot r_3!...}
$$

Example: If there are 12 total items, and 3 share one value, and 5 share another, the total permutations is $\frac{12!}{3!\cdot 5!}$

## Combination

**Combination:** Combination of $r$ items out of a set of $n$ items

Example: In a set of 4 items, there are 6 possible combinations of 2 items.

**Notation:** The total number of combinations is expressed as $_nC_r$

Calculation: Divide $n!$ by the product of $r!$ and $(n-r)!$

Reasoning: In $n!$, each combination is repeated for each combination sequence, which is $r!$, and each of those are repeated for each sequence of the remaining items, which is $(n-r)!$

Formula:

$$
_nC_r = \frac {n!} {r! \cdot (n-r)!}
$$