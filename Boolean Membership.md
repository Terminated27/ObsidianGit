
Boolean membership is a concept in mathematics and computer science that deals with determining whether an element belongs to a [[set]] or not. It is often denoted using the symbol $\in$. In this atomic note, we will explore the key theorems, definitions, and step-by-step examples related to boolean membership.

## Definitions

**[[Set]]**: A [[set]] is a collection of distinct elements. It can be represented by listing its elements inside curly braces. For example, if $A$ is a [[set]] containing elements $a_1$, $a_2$, and $a_3$, it can be written as $A = \{a_1, a_2, a_3\}$.

**Element**: An element is an individual object that belongs to a [[set]]. For example, in the [[set]] $A = \{1, 2, 3\}$, the numbers 1, 2, and 3 are elements of the [[set]].

**Boolean Membership**: Boolean membership refers to the relationship between an element and a [[set]]. If an element belongs to a [[set]], we say that it satisfies boolean membership. This relationship is denoted using the symbol $\in$. For example, if $x$ is an element of [[set]] $A$, we write $x \in A$.

## Theorems

**Theorem 1: Uniqueness of Elements**

In any given [[set]] $A$, each element appears only once. There are no duplicate elements in a [[set]].

**Theorem 2: [[Subset]]**

If every element of [[set]] $A$ is also an element of [[set]] $B$, then we say that $A$ is a [[subset]] of $B$. This relationship can be represented as $A \subseteq B$. Mathematically,

$$
\forall x : (x \in A \implies x \in B)
$$

**Theorem 3: Empty [[Set]]**

The empty [[set]], denoted by $\emptyset$ or $\{\}$, is a [[set]] that contains no elements. It is a [[subset]] of every [[set]].

$$
\forall x : (x \notin \emptyset)
$$

**Theorem 4: Universal [[Set]]**

The universal [[set]], denoted by $U$, is a [[set]] that contains all possible elements. Every [[set]] is a [[subset]] of the universal [[set]].

$$
\forall x : (x \in A)
$$

## Examples

**Example 1:**

Consider the sets $A = \{1, 2, 3\}$ and $B = \{2, 4, 6\}$. Determine whether the element $2$ belongs to each of these sets.

Solution:

For $2$ to belong to a [[set]], it must be an element of that [[set]]. In this case, since $2$ appears in both sets $A$ and $B$, we can say that $2 \in A$ and $2 \in B$.

**Example 2:**

Consider the sets $A = \{1, 2, 3\}$ and $B = \{4, 5\}$. Determine whether the element $6$ belongs to each of these sets.

Solution:

For an element to belong to a [[set]], it must be an element of that [[set]]. In this case, since $6$ does not appear in either sets $A$ or $B$, we can say that $6 \notin A$ and $6 \notin B$.

## Conclusion

Boolean membership provides a way to determine whether an element belongs to a given [[set]] or not. By using the symbol $\in$, we can express this relationship mathematically. Theorems such as uniqueness of elements, [[subset]] relationships, empty sets, and universal sets help us understand and reason about boolean membership.