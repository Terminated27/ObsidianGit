#computing 
[[Partial Orders]]
In mathematics, a **total [[order]]** (or [[linear]] [[order]]) is a binary relation that is reflexive, transitive, antisymmetric, and total. Formally, a total [[order]] on a [[set]] $S$ is a binary relation $\leq$ that satisfies the following properties for all $a,b,c \in S$:

1. **Reflexivity**: $a \leq a$
2. **Transitivity**: If $a \leq b$ and $b \leq c$, then $a \leq c$
3. **Antisymmetry**: If $a \leq b$ and $b \leq a$, then $a = b$
4. **Totality**: For any two elements $a$ and $b$, either $a \leq b$ or $b \leq a$

## Key Theorems

1. **Trichotomy Law**: For any two elements $a$ and $b$ in a totally ordered [[set]], exactly one of the following holds: $a < b$, $a = b$, or $b < a$.

2. **Dedekind Completeness Property**: Every non-empty [[subset]] of a totally ordered [[set]] that is bounded above has a least upper bound.

## Step-by-Step Example

Let's consider the [[set]] of integers $\mathbb{Z}$ with the usual ordering relation $\leq$. 

1. Reflexivity: For any integer $n$, we have $n \leq n$, which satisfies reflexivity.
2. Transitivity: If $m \leq n$ and $n \leq p$, then we also have $m \leq p$, satisfying transitivity.
3. Antisymmetry: If both $m \leq n$ and  $n \leq m$, then we must have  m = n, satisfying antisymmetry.
4. Totality: For any integers m and n, either m ≤ n or n ≤ m holds.

Therefore, the [[set]] of integers with the usual ordering forms a total [[order]].

Total orders play an essential role in various areas of mathematics such as real analysis, [[Graph]] theory, and combinatorics due to their well-defined properties and applications in establishing [[order]] relations between elements in sets.