#math #calculus #stats
# Calculus
The [[Product Rule]] is a fundamental rule in calculus used to find the [[Derivative]] of a product of two functions. It states that if you have two functions, u(x) and v(x), then the [[Derivative]] of their product u(x)v(x) with respect to x is given by:

$$(uv)'=u'*v+u*v'$$

- u′(x): The [[Derivative]] of the first function u(x) with respect to x.
- v′(x): The [[Derivative]] of the second function v(x) with respect to x.

The [[Product Rule]] allows you to differentiate a product of functions by taking the [[Derivative]] of each function individually and then combining them using addition. It is a crucial tool in calculus for finding derivatives of more complex functions.
# Product Rule for [[Conditional Probability]]

The product rule is a fundamental concept in probability theory that allows us to calculate the probability of the intersection of two events given their individual probabilities. In the context of [[conditional probability]], the product rule provides a way to compute the probability of the joint occurrence of two events, given that one [[event]] has already occurred.

## Definition

Let $A$ and $B$ be two events. The product rule states that the [[conditional probability]] of the intersection of events $A$ and $B$, denoted as $P(A \cap B | C)$, where $C$ is another [[event]], is given by:

$$P(A \cap B | C) = P(A | B \cap C) \cdot P(B | C)$$

## Theorem: Law of Total Probability

The law of total probability is a useful theorem that helps in calculating conditional probabilities by considering all possible ways an [[event]] can occur.

Let $B_1, B_2, \ldots, B_n$ be a partition of the [[sample space]] (i.e., mutually exclusive and exhaustive events). Then for any [[event]] $A$, we have:

$$P(A) = \sum_{i=1}^{n} P(A | B_i) \cdot P(B_i)$$

## Example

Suppose we have two urns: Urn 1 contains 3 red balls and 2 blue balls, while Urn 2 contains 4 red balls and 3 blue balls. We randomly select an urn with equal probability and then draw a ball from it.

Let's define the following events:
- $R$: The selected urn is Urn 1.
- $B$: The selected urn is Urn 2.
- $Red$: A red ball is drawn.
- $Blue$: A blue ball is drawn.

We are interested in finding the [[conditional probability]] that a red ball is drawn, given that Urn 1 was selected.

Using the product rule, we have:

$$P(Red \cap R) = P(Red | R) \cdot P(R)$$

The probability of drawing a red ball given that Urn 1 was selected is $\frac{3}{5}$, as there are 3 red balls out of a total of 5 balls in Urn 1. The probability of selecting Urn 1 is $\frac{1}{2}$, as both urns are equally likely to be chosen.

Therefore, we can calculate:

$$P(Red \cap R) = \left(\frac{3}{5}\right) \cdot \left(\frac{1}{2}\right) = \frac{3}{10}$$

Hence, the [[conditional probability]] of drawing a red ball given that Urn 1 was selected is $\frac{3}{10}$.

## Conclusion

The product rule for [[conditional probability]] provides a way to compute the joint probability of two events given the conditional probabilities. It is a fundamental concept in probability theory and finds applications in various fields such as [[Statistics equations]], [[machine learning]], and decision theory. Understanding and applying the product rule allows us to reason about uncertain events and make informed decisions based on available information.