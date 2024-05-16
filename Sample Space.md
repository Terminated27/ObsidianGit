#math #stats

In probability theory, a **sample space** is the [[set]] of all possible outcomes of an experiment. It is denoted by the symbol $\Omega$.

## Definition

Formally, a sample space is defined as a non-empty [[set]] that contains all possible outcomes of an experiment. Each outcome in the sample space is called an **elementary [[event]]** or a **sample point**.

## Example

Consider flipping a fair coin. The sample space for this experiment consists of two possible outcomes: {Heads, Tails}. Therefore, $\Omega = \{H, T\}$.

## Cardinality of Sample Space

The **cardinality** (size) of a sample space $\Omega$ is denoted by $|\Omega|$. For a finite sample space, $|\Omega|$ represents the number of possible outcomes.

## Example

In the coin flipping example, $|\Omega| = 2$ since there are two possible outcomes (Heads and Tails).

## Events and Subsets

An **event** is any [[subset]] of the sample space. It represents a collection of possible outcomes. Events can be simple (consisting of only one outcome) or compound (consisting of multiple outcomes).

## Example

Consider flipping two fair coins. Some examples of events are:
- Getting at least one Head: {HH, HT, TH}
- Getting exactly one Tail: {HT, TH}

## Operations on Events

### Union ($\cup$)

The union of two events $A$ and $B$, denoted by $A \cup B$, consists of all outcomes that belong to either [[event]] $A$, [[event]] $B$, or both.

### Intersection ($\cap$)

The intersection of two events $A$ and $B$, denoted by $A \cap B$, consists of all outcomes that belong to both [[event]] $A$ and [[event]] $B$.

### Complement ($A^c$)

The complement of an [[event]] $A$, denoted by $A^c$, consists of all outcomes that do not belong to [[event]] $A$.

### Mutually Exclusive Events

Two events $A$ and $B$ are said to be mutually exclusive (or disjoint) if their intersection is an empty [[set]], i.e., $A \cap B = \emptyset$. This means that the occurrence of one [[event]] excludes the occurrence of the other.

## Probability of an [[Event]]

The probability of an [[event]] $A$, denoted by $P(A)$, is a measure of the likelihood that [[event]] $A$ will occur. It is a number between 0 and 1 (inclusive).

## Key Theorems

### Theorem 1: Probability Axioms

For any [[event]] $A$ in a sample space $\Omega$, the following axioms hold:

1. Non-negativity: $P(A) \geq 0$
2. Normalization: $P(\Omega) = 1$
3. Additivity: For any sequence of mutually exclusive events $(A_1, A_2, \ldots)$, we have $$P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i)$$

### Theorem 2: Complement Rule

For any [[event]] $A$ in a sample space $\Omega$, we have $$P(A^c) = 1 - P(A)$$

### Theorem 3: Union Rule

For any two events $A$ and $B$ in a sample space $\Omega$, we have $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$