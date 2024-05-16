

In probability theory, **marginal probability** refers to the probability of a single [[event]] occurring without considering any other events. It is obtained by summing or integrating the joint probability distribution over all other variables except the one of interest.

## Definition
The marginal probability of an [[event]] A can be calculated as:

$$ P(A) = \sum_{B} P(A,B) $$

where $P(A,B)$ is the joint probability of events A and B.

## Theorem: Law of Total Probability
The law of total probability states that for any partition {B1, B2, ..., Bn} of the [[sample space]] S, we have:

$$ P(A) = \sum_{i=1}^{n} P(A|B_i)P(B_i) $$

where $P(A|B_i)$ is the [[conditional probability]] of [[event]] A given [[event]] Bi.
what is n here


## Example
Consider a random experiment where a fair six-sided die is rolled. Let A be the [[event]] that the outcome is an even number (2, 4, or 6), and B be the [[event]] that the outcome is greater than 3 (4, 5, or 6).

The joint probabilities are:
- $P(A \cap B) = P(\{4, 6\}) = \frac{2}{6} = \frac{1}{3}$
- $P(A) = P(\{2, 4, 6\}) = \frac{3}{6} = \frac{1}{2}$
- $P(B) = P(\{4, 5, 6\}) = \frac{3}{6} = \frac{1}{2}$

Using the law of total probability:
$$ P(A) = P(A|B)P(B) + P(A|\neg B)P(\neg B) $$

Substitute in the known values:
$$ P(A) = \frac{1}{3}\cdot\frac{1}{2} + \frac{1}{2}\cdot\frac{1}{2} = \frac{1}{6} + \frac{1}{4} = \frac{5}{12} $$

Therefore, the marginal probability of rolling an even number on a fair six-sided die is $\frac{5}{12}$.

By understanding marginal probabilities and utilizing tools like the law of total probability, we can analyze complex systems and make informed decisions based on probabilistic outcomes.