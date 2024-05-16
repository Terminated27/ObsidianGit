#math 


# Subset

In [[set]] theory, a **subset** is a collection of elements that are all contained within another [[set]]. More formally, if every element of [[set]] A is also an element of [[set]] B, then A is said to be a subset of B, denoted as $A \subseteq B$. 

## Definition

Let A and B be sets. A is a subset of B if and only if every element of A is also an element of B. This can be mathematically represented as:

$$
A \subseteq B \iff (\forall x)(x \in A \implies x \in B)
$$

## Example

Consider two sets:

$A = \{1, 2, 3\}$ and $B = \{1, 2, 3, 4\}$.

Here, every element in [[set]] A (1, 2, and 3) is also present in [[set]] B. Therefore, we can say that A is a subset of B: $A \subseteq B$.

## Proper Subset

If every element in [[set]] A is also an element in [[set]] B but there exists at least one element in [[set]] B that is not present in [[set]] A, then we say that A is a **proper subset** of B. This is denoted as $A \subset B$.

## Example

Consider two sets:

$C = \{1, 2\}$ and $D = \{1, 2, 3\}$.

Here, every element in C (1 and 2) is also present in D. However, D contains an additional element (3) that does not belong to C. Therefore, we can say that C is a proper subset of D: $C \subset D$.

## Cardinality of Subsets

The **cardinality** of a [[set]] refers to the number of elements in that [[set]]. For a given [[set]] A, the cardinality of A is denoted as $|A|$. 

If A is a finite [[set]], then the cardinality of A can be determined by counting the number of elements in A. For example, if $A = \{1, 2, 3\}$, then $|A| = 3$.

For subsets, the cardinality of a subset A is always less than or equal to the cardinality of its superset B. Mathematically:

$$
A \subseteq B \implies |A| \leq |B|
$$

## [[Power]] [[Set]]

The **[[power]] [[set]]** of a [[set]] A is the collection of all possible subsets of A. It is denoted as $\mathcal{P}(A)$.

For a given [[set]] with n elements, the [[power]] [[set]] will contain $2^n$ subsets.

## Example

Consider a [[set]]:

$E = \{a, b\}$.

The [[power]] [[set]] $\mathcal{P}(E)$ will contain all possible subsets of E:

$\mathcal{P}(E) = \{\{\}, \{a\}, \{b\}, \{a, b\}\}$.

Here, $\{\}$ represents the empty [[set]] and $\{a, b\}$ represents the original [[set]] E itself.

## Conclusion

Understanding subsets is fundamental in [[set]] theory. It allows us to compare and analyze relationships between sets based on their elements. The concept of proper subsets further refines this comparison by considering strict containment. Additionally, knowing the cardinality and [[power]] sets provides valuable insights into the size and structure of sets.