#stats 

Ordered sampling is a statistical technique that involves selecting a sample from a population in a specific [[order]]. In ordered sampling, the [[order]] in which the elements are selected is important and can affect the results of the analysis. This technique is commonly used in various fields, including market research, quality control, and experimental design.

## Definitions

**Ordered Sample**: An ordered sample is a [[subset]] of elements selected from a population in a specific [[order]].

**Ordered Sampling**: Ordered sampling is the process of selecting an ordered sample from a population.

## Key Theorems

### Theorem 1: Number of Ordered Samples without Replacement

The number of possible ordered samples without replacement from a population of size $N$, when selecting $n$ elements at a time, is given by:

$$
\frac{{N!}}{{(N-n)!}}
$$

### Theorem 2: Number of Ordered Samples with Replacement

The number of possible ordered samples with replacement from a population of size $N$, when selecting $n$ elements at a time, is given by:

$$
N^n
$$

## Examples

### Example 1: Ordered Sampling without Replacement

Suppose we have a deck of playing cards with 52 cards. We want to select 3 cards at random without replacement. How many different ordered samples can we obtain?

Using Theorem 1, we can calculate the number of possible ordered samples without replacement as:

$$
\frac{{52!}}{{(52-3)!}} = \frac{{52!}}{{49!}} = 52 \times 51 \times 50 = 132,600
$$

Therefore, there are 132,600 different ordered samples that can be obtained by selecting 3 cards from the deck.

### Example 2: Ordered Sampling with Replacement

Consider an urn containing red and blue balls. There are 5 red balls and 3 blue balls in the urn. We want to select 2 balls at random with replacement. How many different ordered samples can we obtain?

Using Theorem 2, we can calculate the number of possible ordered samples with replacement as:

$$
(5+3)^2 = 8^2 = 64
$$

Therefore, there are 64 different ordered samples that can be obtained by selecting 2 balls from the urn with replacement.

## Conclusion

Ordered sampling is a useful technique in statistics that allows us to select a sample from a population in a specific [[order]]. The number of possible ordered samples depends on whether sampling is done with or without replacement. Theorems 1 and 2 provide formulas for calculating the number of possible ordered samples in each case. By understanding and applying these concepts, researchers can make informed decisions when designing experiments or conducting analyses that involve ordered sampling.