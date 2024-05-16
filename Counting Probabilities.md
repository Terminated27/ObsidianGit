#stats 

Counting probabilities is a fundamental concept in probability theory that involves determining the number of favorable outcomes and total possible outcomes in a given scenario to calculate the probability of an [[event]] occurring.

## Permutations and Combinations

### Permutations

A permutation refers to an arrangement of objects in a specific [[order]]. The number of permutations of n distinct objects taken r at a time is given by:

$$ P(n, r) = \frac{n!}{(n-r)!} $$

where $n!$ denotes the factorial of n.

### Combinations

A combination represents a selection of objects without considering the [[order]]. The number of combinations of n distinct objects taken r at a time is calculated as:

$$ C(n, r) = \binom{n}{r} = \frac{n!}{r!(n-r)!} $$

## Probability Calculation using Counting Techniques

To calculate the probability of an [[event]] using counting techniques, we can use the following formula:

$$ P(A) = \frac{\text{Number of favorable outcomes}}{\text{Total possible outcomes}} $$

### Example: Rolling Two Dice

Consider rolling two fair six-sided dice. Let A be the [[event]] that the sum of the numbers rolled is 7. 

1. **Favorable Outcomes**: There are 6 ways to get a sum of 7: (1,6), (2,5), (3,4), (4,3), (5,2), (6,1).
2. **Total Possible Outcomes**: Since each die has 6 sides, there are $6 \times 6 = 36$ total outcomes.

Therefore, the probability of [[event]] A occurring is:

$$ P(A) = \frac{6}{36} = \frac{1}{6} $$

By applying counting techniques like permutations and combinations, we can efficiently determine probabilities in various scenarios.