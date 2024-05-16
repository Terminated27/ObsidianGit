#math
A set is a fundamental concept in mathematics that represents a collection of distinct objects. These objects are called elements or members of the set. Sets are widely used in various branches of mathematics, including algebra, calculus, and probability theory.

## Notation

Sets are typically denoted using capital letters. If an element belongs to a set, it is denoted using lowercase letters. For example, if "a" is an element of set "A," we write $a \in A$. Conversely, if an element does not belong to a set, we write $b \notin A$.

## Set Builder Notation

Set builder notation is a concise way to describe sets using properties or conditions that the elements must satisfy. It has the form $\{x \mid P(x)\}$, where $x$ represents the elements and $P(x)$ is a predicate that defines the condition for membership.

For example, let's define a set $E$ containing even numbers less than 10:

$$E = \{x \mid x \text{ is an even number and } x < 10\}$$

In this case, $E$ can be written as $E = \{2, 4, 6, 8\}$.

## [[Set Operations]]

Sets can be combined or manipulated using various operations. Let's discuss some key operations:

[[Subset]]
### Union ($\cup$) (OR)

The union of two sets $A$ and $B$, denoted by $A \cup B$, is the set that contains all elements from both sets without duplication.
**Keyword: OR**

For example:
- If $A = \{1, 2\}$ and $B = \{2, 3\}$,
- Then $A \cup B = \{1, 2, 3\}$.

### Intersection ($\cap$) (AND)

The intersection of two sets $A$ and $B$, denoted by $A \cap B$, is the set that contains elements common to both sets.
**Keyword: AND**

For example:
- If $A = \{1, 2\}$ and $B = \{2, 3\}$,
- Then $A \cap B = \{2\}$.

### Difference ($-$)

The difference of two sets $A$ and $B$, denoted by $A - B$, is the set that contains elements from set $A$ but not in set $B$.
**Keyword: NOT**

For example:
- If $A = \{1, 2, 3\}$ and $B = \{2, 3\}$,
- Then $A - B = \{1\}$.

### Complement ($'$ or $\overline{A}$) (NOT)

The complement of a set $A$, denoted by either $A'$ or $\overline{A}$, is the set that contains all elements not in set $A$. The universal set (denoted by $\Omega$) is the set of all possible elements in a given context.

For example:
- If $\Omega$ is the universal set and $A = \{1, 2\}$,
- Then $\overline{A} = \Omega - A$ (complement of A with respect to $\Omega$).
### Relative Complement (Set Minus) ($A \setminus B$)

The relative complement of a set $B$ in relation to another set $A$, denoted by $A \setminus B$, is the set of elements that are in $A$ but not in $B$.
**Keyword: NOT IN B**

For example:
- If $A = \{1, 2, 3, 4\}$ and $B = \{3, 4, 5\}$,
- Then $A \setminus B = \{1, 2\}$.

Another way to interpret the relative complement is to consider it as the part of $A$ that "remains" after removing the elements that are also in $B$.

The relative complement can be expressed mathematically as:
$A \setminus B = \{x \in A \,|\, x \notin B\}$

Relative complement is sometimes referred to as set minus because it computes the difference between sets.

### Symmetric Difference ($\triangle$) (XOR)

The symmetric difference of two sets $A$ and $B$, denoted by $A \triangle B$, is the set of elements that are in either of the sets, but not in their intersection.

For example:
- If $A = \{1, 2, 3\}$ and $B = \{2, 3, 4\}$,
- Then $A \triangle B = \{1, 4\}$.

Another way to think about the symmetric difference is to consider it as the set of elements that are in one of the sets, but not in both.

The symmetric difference can be computed using the following formula:
$A \triangle B = (A - B) \cup (B - A)$

This operation essentially captures the elements that are exclusive to each set. It is called "symmetric" because the result is the same regardless of the order of the sets.

Symmetric difference is particularly useful in various areas, including set theory, computer science, and cryptography, where it helps in determining elements that are unique to each set while excluding those that are common.
### Disjoint Sets

Two sets $A$ and $B$ are said to be disjoint if they have no elements in common, or equivalently, their intersection is the empty set.

For example:
- If $A = \{1, 2\}$ and $B = \{3, 4\}$,
- Then $A$ and $B$ are disjoint because $A \cap B = \emptyset$.

Another way to understand disjoint sets is to consider them as sets that do not share any elements; they are entirely separate from each other.

Disjoint sets can be represented symbolically as:

- If $A \cap B = \emptyset$, then $A$ and $B$ are disjoint.

Disjoint sets are crucial in various mathematical concepts, such as probability theory, where events are often considered disjoint if they cannot occur simultaneously.

### [[Subset]] ($\subseteq$)

a [[subset]] is a collection of elements that are all contained within another set. More formally, if every element of set A is also an element of set B, then A is said to be a [[subset]] of B, denoted as $A \subseteq B$. 

For example: 
* $A = \{1, 2, 3\}$ and $B = \{1, 2, 3, 4\}$.
* every element in set A (1, 2, and 3) is also present in set B. Therefore, $A \subseteq B$.
## Set Cardinality

The cardinality of a set refers to the number of elements it contains. It can be denoted using vertical bars around the set: $\lvert A \rvert$. For example, if we have a set $C = \{a, b, c\}$, then $\lvert C \rvert = 3$.

## Key Theorems

### De Morgan's Laws

De Morgan's Laws describe how logical operations on sets can be expressed using complements. Let's consider two sets $A$ and $B$:

1. The complement of the union of sets $A$ and $B$ is equal to the intersection of their complements: $(A \cup B)' = A' \cap B'$.
2. The complement of the intersection of sets $A$ and $B$ is equal to the union of their complements: $(A \cap B)' = A' \cup B'$.

These laws are useful for simplifying set expressions and proving set identities.
### The Null set

The null set is any empty set, it is denoted by  $\phi$
For example:
* $A = \{ \space \} = ∅$
## Examples

### Example 1: [[Set Operations]]

Consider the following sets:
- $A = \{1, 2, 3\}$
- $B = \{2, 3, 4\}$
- $C = \{3, 4, 5\}$

Let's perform some [[set operations]]:

1. Find $A \cup B$: 
   - $A \cup B = \{1, 2, 3\} \cup \{2, 3, 4\}$
   - $A \cup B = \{1, 2, 3, 4\}$

2. Find $(A - B) \cap C$: 
   - $(A - B) = A - (B) = A - (B \cap C)$
   - $(A - B) = A - (2)$
   - $(A - B) = A$
   - $(A - B) \cap C = A \cap C$
   - $(A - B) \cap C = (\{1, 2, 3\}) \cap (\{3, 4, 5\})$
   - $(A - B) \cap C = (\{3\})$
   
### Example 2: De Morgan's Laws

Let's use De Morgan's Laws to simplify the following set expression:

$(A \cup B)' \cap C'$

1. Apply De Morgan's Law 1:
   - $(A \cup B)' = A' \cap B'$
   
2. Simplify the expression:
   - $(A' \cap B') \cap C'$
   - $A' \cap (B' \cap C')$
   - $A' \cap (B \cup C)'$

The simplified expression is $A' \cap (B \cup C)'$.

These examples demonstrate how [[set operations]] and theorems can be applied to solve problems and manipulate sets.

This atomic note provides a comprehensive overview of sets, including notation, set builder notation, [[set operations]], complement, cardinality, and key theorems like De Morgan's Laws. The examples illustrate the practical application of these concepts.