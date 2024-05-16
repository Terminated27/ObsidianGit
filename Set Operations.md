#math #stats 

In [[set]] theory, various operations can be performed on sets to generate new sets. These operations include union, intersection, difference, and complement. This atomic note will provide a detailed explanation of these [[set]] operations.

## Union of Sets

The union of two sets A and B, denoted by $A \cup B$, is the [[set]] that contains all elements present in either A or B or both. In other words, it is the combination of all distinct elements from both sets.

$$
A \cup B = \{x : x \in A \text{ or } x \in B\}
$$

### Properties of Union
1. Commutative Property: $A \cup B = B \cup A$
2. Associative Property: $(A \cup B) \cup C = A \cup (B \cup C)$
3. Identity Property: $A \cup \varnothing = A$
4. Idempotent Property: $A \cup A = A$

## Intersection of Sets

The intersection of two sets A and B, denoted by $A \cap B$, is the [[set]] that contains all elements present in both A and B.

$$
A \cap B = \{x : x\in A  \text{ and } x\in B\}
$$

### Properties of Intersection
1. Commutative Property: $A\cap B = B\cap A$
2. Associative Property: $(A\cap B)\cap C = A\cap (B\cap C)$
3. Identity Property: $A\cap U = A$
4. Idempotent Property: $A\cap A = A$

## Difference of Sets

The difference between two sets A and B, denoted by $A - B$ or $A\setminus B$, is the [[set]] that contains all elements present in A but not in B.

$$
A - B = \{x : x\in A  \text{ and } x\notin B\}
$$

### Properties of Difference
1. $A - B \neq B - A$ (Difference is not commutative)
2. $A - (B - C) = (A - B) \cup (A - C)$

## Complement of a [[Set]]

The complement of a [[set]] A with respect to a universal [[set]] U, denoted by $A'$ or $\overline{A}$, is the [[set]] that contains all elements present in U but not in A.

$$
A' = \{x : x\in U  \text{ and } x\notin A\}
$$

### Properties of Complement
1. $(A')' = A$
2. $U' = \varnothing$
3. $\varnothing ' = U$

## Examples

Let's consider the following sets:

$A = \{1, 2, 3\}$ and $B = \{2, 3, 4\}$.

1. Union: $A \cup B = \{1, 2, 3, 4\}$
2. Intersection: $A \cap B = \{2, 3\}$
3. Difference: $A - B = \{1\}$ and $B - A = \{4\}$
4. Complement: If the universal [[set]] is $U = \{1, 2, 3, 4, 5\}$,
   * $A' = U - A = \{4, 5\}$
   * $B' = U - B = \{1, 5\}$