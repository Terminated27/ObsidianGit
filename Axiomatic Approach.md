#stats 
# Statistics

The axiomatic approach is a fundamental framework used in statistics to establish the foundations of the discipline. It provides a [[set]] of axioms, or basic assumptions, from which all statistical theories and methods can be derived. In this atomic note, we will discuss the key axioms and their implications in statistics.

## Axioms

### Axiom 1: [[Sample Space]]

The [[sample space]], denoted by $\Omega$, is the [[set]] of all possible outcomes of an experiment. It is assumed to be non-empty and finite or countably infinite.

### Axiom 2: Events

An [[event]] is a [[subset]] of the [[sample space]]. We denote events by capital letters such as $A$, $B$, etc. The empty [[set]] $\emptyset$ and the [[sample space]] $\Omega$ are considered events.

### Axiom 3: Probability Measure

A probability measure $P$ assigns a real number between 0 and 1 to each [[event]] in the [[sample space]]. It satisfies the following properties:

1. Non-negativity: $P(A) \geq 0$ for any [[event]] $A$.
2. Normalization: $P(\Omega) = 1$.
3. [[Countable]] Additivity: For any sequence of mutually exclusive events $A_1, A_2, \ldots$, i.e., $A_i \cap A_j = \emptyset$ for $i \neq j$, we have $$P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i).$$ $$
P(A \text{ or } B) = P(A) + P(B)
$$
These axioms provide a solid foundation for probability theory and allow us to reason about uncertainty in a rigorous manner.

## Theorems

### Theorem 1: Complement Rule

For any [[event]] $A$, the probability of the complement of $A$ is given by $$P(A^c) = 1 - P(A).$$

### Theorem 2: Union Rule

For any two events $A$ and $B$, the probability of their union is given by $$P(A \cup B) = P(A) + P(B) - P(A \cap B).$$

### Theorem 3: Inclusion-Exclusion Principle

For any finite sequence of events $A_1, A_2, \ldots, A_n$, the probability of their union is given by $$P\left(\bigcup_{i=1}^{n} A_i\right) = \sum_{i=1}^{n} P(A_i) - \sum_{i < j} P(A_i \cap A_j) + \sum_{i < j < k} P(A_i \cap A_j \cap A_k) - \ldots + (-1)^{n+1} P(A_1 \cap A_2 \cap \ldots \cap A_n).$$

This theorem allows us to compute the probability of complex events involving multiple unions and intersections.

## Example

Consider a fair six-sided die. Let's define two events:

- [[Event]] $A$: Rolling an odd number.
- [[Event]] $B$: Rolling a number less than or equal to 3.

We can use the axioms and theorems to compute probabilities associated with these events.

From Axiom 3, we know that each outcome (rolling a specific number) has equal probability $\frac{1}{6}$ since it is a fair die. Therefore, we have:

$$P(A) = P(\{1, 3, 5\}) = \frac{3}{6} = \frac{1}{2},$$
$$P(B) = P(\{1, 2, 3\}) = \frac{3}{6} = \frac{1}{2}.$$

Using Theorem 2, we can compute the probability of their union:

$$P(A \cup B) = P(\{1, 2, 3, 5\}) = \frac{4}{6} = \frac{2}{3}.$$

This example demonstrates how the axiomatic approach allows us to reason about probabilities using basic assumptions and [[logical rules]].

In conclusion, the axiomatic approach provides a solid foundation for statistics by defining the [[sample space]], events, and probability measure. Theorems derived from these axioms allow us to compute probabilities of various events and make informed decisions based on statistical analysis.