#computing 
[[Total Orders]]
In mathematics, a **partial [[order]]** is a binary relation that is reflexive, antisymmetric, and transitive. Formally, a partial [[order]] on a [[set]] $S$ is a relation $\leq$ that satisfies the following properties for all $a, b, c \in S$:

1. Reflexivity: $a \leq a$
2. Antisymmetry: If $a \leq b$ and $b \leq a$, then $a = b$
3. Transitivity: If $a \leq b$ and $b \leq c$, then $a \leq c$

A partial [[order]] can be represented by a directed acyclic [[Graph]] where the elements of the [[set]] are nodes and there is an edge from [[node]] $a$ to [[node]] $b$ if and only if $a \leq b$. 

## Hasse Diagram

A **Hasse diagram** is a graphical representation of a partial [[order]] showing the elements as nodes and the ordering relation as edges. It is drawn in such a way that if there is an edge from [[node]] $a$ to [[node]] $b$, then $a < b$ and there are no unnecessary edges.

## Example

Consider the [[set]] $\{1, 2, 3\}$ with the partial [[order]] defined by $\{(1, 1), (1, 2), (1, 3), (2, 2), (3, 3)\}$. The Hasse diagram for this partial [[order]] would be:

```
   3
   |
   1
   |
   2
```

In this example, we see that $1 < 2$, $1 < 3$, but there is no direct relation between 2 and 3.

## Key Theorems

### Maximal Element
An element $m$ in a partially ordered [[set]] $(S,\leq)$ is called **maximal** if there does not exist any element in $S$ greater than or equal to $m$. Formally,
$$\forall x \in S : m \leq x \implies m = x$$

### Minimal Element
An element $\mu$ in a partially ordered [[set]] $(S,\leq)$ is called **minimal** if there does not exist any element in $S$ less than or equal to $\mu$. Formally,
$$\forall x \in S : x \leq \mu \implies x = \mu$$

### Lattice
A **lattice** is a partially ordered [[set]] in which every pair of elements has both a supremum (least upper bound) and an infimum (greatest lower bound).

Partial orders play an important role in various branches of mathematics such as algebraic structures and combinatorics. Understanding partial orders helps in analyzing relationships between elements within sets.