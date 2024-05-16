#math #stats 

Conditional probability is a fundamental concept in probability theory that measures the likelihood of an [[event]] occurring given that another [[event]] has already occurred. It provides a way to update our beliefs about the occurrence of an [[event]] based on new information.

## Definition

The conditional probability of an [[event]] A given that [[event]] B has occurred is denoted by $P(A|B)$ and is defined as:

$$P(A|B) = \frac{P(A \cap B)}{P(B)},$$

where $P(A \cap B)$ represents the probability of both events A and B occurring simultaneously, and $P(B)$ represents the probability of [[event]] B occurring.

## Theorem: Multiplication Rule

The multiplication rule allows us to calculate the probability of the intersection of two events. For any two events A and B, it states:

$$P(A \cap B) = P(A|B) \cdot P(B).$$

This theorem follows directly from the definition of conditional probability.

## Theorem: Law of Total Probability

The law of total probability states that for any partition $\{B_1, B_2, \ldots, B_n\}$ of the [[sample space]] S (i.e., a collection of mutually exclusive and exhaustive events), we have:

$$P(A) = \sum_{i=1}^{n} P(A|B_i) \cdot P(B_i),$$

where A is any [[event]] in the [[sample space]] S.

This theorem allows us to express the probability of an [[event]] A in terms of conditional probabilities.

## Example 1: Coin Tossing

Consider tossing two fair coins. Let's define two events:
- A: Getting at least one head
- B: Getting exactly one head

We want to find $P(A|B)$, i.e., the probability of getting at least one head given that exactly one head has been obtained.

To solve this problem, we need to find $P(A \cap B)$ and $P(B)$.

The [[event]] A can occur in two ways: (1) getting a head on the first coin and a tail on the second coin, or (2) getting a tail on the first coin and a head on the second coin. Each of these possibilities has a probability of $\frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4}$. Therefore, $P(A \cap B) = 2 \cdot \frac{1}{4} = \frac{1}{2}$.

The [[event]] B can only occur in one way: getting a head on the first coin and a tail on the second coin. Thus, $P(B) = \frac{1}{4}$.

Using the definition of conditional probability, we have:

$$P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{\frac{1}{2}}{\frac{1}{4}} = 2.$$

Therefore, the probability of getting at least one head given that exactly one head has been obtained is 2.

## Example 2: Medical Test

Suppose there is a medical test for detecting a certain disease. Let's define two events:
- A: Having the disease
- B: Testing positive for the disease

We are given that the test correctly identifies 95% of people who have the disease (i.e., $P(B|A) = 0.95$), and it incorrectly identifies 3% of people who do not have the disease (i.e., $P(B|\neg A) = 0.03$). We also know that only 0.5% of the population actually has the disease (i.e., $P(A) = 0.005$).

We want to find $P(A|B)$, i.e., the probability of having the disease given that the test is positive.

Using Bayes' theorem, we have:

$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}.$$

To calculate $P(B)$, we can use the law of total probability:

$$P(B) = P(B|A) \cdot P(A) + P(B|\neg A) \cdot P(\neg A).$$

Since $P(\neg A) = 1 - P(A)$, we have:

$$P(B) = P(B|A) \cdot P(A) + P(B|\neg A) \cdot (1 - P(A)).$$

Substituting the given values, we get:

$$P(B) = 0.95 \cdot 0.005 + 0.03 \cdot (1 - 0.005).$$

Now, we can calculate $P(A|B)$:

$$P(A|B) = \frac{0.95 \cdot 0.005}{0.95 \cdot 0.005 + 0.03 \cdot (1 - 0.005)}.$$

Simplifying this expression gives us the desired conditional probability.

## Conclusion

Conditional probability is a powerful tool for reasoning about uncertain events in light of new information or conditions. It allows us to update our beliefs and make more informed decisions based on available evidence. The multiplication rule and the law of total probability are key theorems that help us compute conditional probabilities in various scenarios.

Remember to always carefully define events and consider all relevant probabilities when applying conditional probability concepts to real-world situations.
