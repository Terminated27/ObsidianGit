#math #stats 
Conditional independence is a fundamental concept in probability theory and [[Statistics equations]]. It allows us to express the relationship between [[multiple random variables]] in terms of conditional probabilities. In this atomic note, we will explore the definition of conditional independence, discuss key theorems related to it, and provide step-by-step examples to illustrate its application.

## Definition

Let's consider three random variables: A, B, and C. We say that A is **conditionally independent** of B given C if the [[conditional probability]] distribution of A given both B and C is equal to the [[conditional probability]] distribution of A given C alone. Mathematically, this can be expressed as:

$$P(A | B,C) = P(A | C)$$

This equation implies that knowledge about B does not provide any additional information about A beyond what is already known from C alone.

## Key Theorems

### Theorem 1: Chain Rule for [[Conditional Probability]]

The chain rule for [[conditional probability]] states that any joint probability distribution can be expressed as a product of conditional probabilities. For three random variables A, B, and C, it can be written as:

$$P(A,B,C) = P(A | B,C) \cdot P(B | C) \cdot P(C)$$

### Theorem 2: [[Product Rule]] for Conditional Independence

The [[product rule]] for conditional independence allows us to express the joint probability distribution of two conditionally independent random variables in terms of their individual conditional probabilities. For three random variables A, B, and C:

If A is conditionally independent of B given C and D is conditionally independent of B given C, then:

$$P(A,B | C) = P(A | C) \cdot P(B | C)$$

### Theorem 3: Bayes' Rule for Conditional Independence

Bayes' rule can also be extended to incorporate conditional independence relationships. For three random variables A, B, and C:

If A is conditionally independent of B given C, then:

$$P(A | B,C) = \frac{P(B | A,C) \cdot P(A | C)}{P(B | C)}$$

## Examples

Let's consider a simple example to understand conditional independence better.

Example 1: Flipping Coins

Suppose we have three fair coins: A, B, and C. Let A represent the outcome of the first coin flip, B represent the outcome of the second coin flip, and C represent the outcome of the third coin flip.

We can define three events: H (heads) and T (tails). Each coin flip has two possible outcomes: H or T.

Given that we know the outcome of the first coin flip (A), does knowing the outcome of the second coin flip (B) provide any additional information about the outcome of the third coin flip (C)?

Intuitively, we can see that knowing whether the first coin landed on heads or tails does not affect our knowledge about whether the third coin will land on heads or tails. Therefore, we can say that A is conditionally independent of C given B.

Mathematically:

$$P(C | A,B) = P(C | B)$$

This example illustrates how conditional independence allows us to simplify complex probability distributions by reducing dependencies between random variables.

## Conclusion

Conditional independence is a powerful concept in probability theory that allows us to express relationships between random variables in terms of conditional probabilities. It provides a way to simplify complex probability distributions by reducing dependencies. The key theorems presented in this atomic note help formalize and apply conditional independence in various scenarios. Understanding conditional independence is crucial for many statistical models and inference techniques.