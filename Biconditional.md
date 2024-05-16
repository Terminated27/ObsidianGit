#compnum 

The biconditional, denoted by $\iff$, is a logical connective that represents a two-way [[implication]]. It is true when both statements have the same truth value, either both true or both false.

## Definition
The biconditional statement $P \iff Q$ is true if and only if $P$ and $Q$ have the same truth value.

## Theorems
1. **Biconditional Equivalence**: The biconditional $P \iff Q$ is equivalent to $(P \rightarrow Q) \land (Q \rightarrow P)$.
   
   $$P \iff Q \equiv (P \rightarrow Q) \land (Q \rightarrow P)$$

2. **Negation of Biconditional**: The negation of $P \iff Q$ is equivalent to $(P \land \lnot Q) \lor (\lnot P \land Q)$.

   $$\lnot (P \iff Q) = (P \land \lnot Q) \lor (\lnot P \land Q)$$

## Truth table

| p | q | p ↔ q |
|---|---|-------|
| T | T |   T   |
| T | F |   F   |
| F | T |   F   |
| F | F |   T   |