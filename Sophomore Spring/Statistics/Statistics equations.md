#stats 
# Equations
 Probability can be expressed using sets, particularly in the context of [[Set Operations]]. Here are some common equations related to probability using sets:
### Union of Events ($A \cup B$)

The union of two events $A$ and $B$ represents the [[event]] that either $A$ or $B$ (or both) occurs.

$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

### Intersection of Events ($A \cap B$)

The intersection of two events $A$ and $B$ represents the [[event]] that both $A$ and $B$ occur.

$$
P(A \cap B) = P(A) \times P(B \mid A)
$$

### Complement of an [[Event]] ($A'$ or $\overline{A}$)

The complement of an [[event]] $A$ represents the [[event]] that $A$ does not occur.

$$
P(A') = 1 - P(A)
$$

### [[Conditional Probability]] ($P(B \mid A)$)

[[Conditional probability]] represents the probability of [[event]] $B$ occurring given that [[event]] $A$ has already occurred.

$$
P(B \mid A) = \frac{P(A \cap B)}{P(A)}
$$

### Independence of Events

Two events $A$ and $B$ are independent if the occurrence of one [[event]] does not affect the occurrence of the other.

$$
P(A \cap B) = P(A) \times P(B)
$$

### Total Probability Theorem

The total probability theorem expresses the probability of an [[event]] in terms of conditional probabilities and the probabilities of related events.

$$
P(B) = \sum_{i} P(A_i) \times P(B \mid A_i)
$$

where $\{A_i\}$ is a partition of the [[sample space]].
### Bayes' Theorem

Bayes' theorem relates the [[conditional probability]] of an [[event]] given prior knowledge to the [[conditional probability]] of the prior knowledge given the [[event]].

$$
P(A \mid B) = \frac{P(B \mid A) \times P(A)}{P(B)}
$$
### Bayes' Theorem for Multiple Hypotheses

When there are multiple hypotheses $A_1, A_2, \ldots, A_n$ and a new piece of evidence $B$ is observed, Bayes' theorem can be extended to consider each hypothesis: 

$$
P(A_i \mid B) = \frac{P(B \mid A_i) \times P(A_i)}{\sum_{i=1}^{n} P(B \mid A_i) \times P(A_i)}
$$
[[Discrete Random Variable]]
[[Cumulative Distribution Function]]
[[Expected Values]]
[[Continuous Random Variable]]
[[Random Variable]]
[[Poisson Random Variable]]
[[Gaussian Random Variable]]

USE EQUATIONS FROM THIS ON CRIB SHEET