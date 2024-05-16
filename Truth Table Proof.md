#math 
## Definition

A truth table is a table that shows the possible values of a logical expression for each combination of truth values of its variables. It is used to determine the validity of a logical argument or to evaluate the truth value of a compound proposition.

## Theorem: Completeness of Truth Tables

Every well-formed formula in [[propositional logic]] can be proven using truth tables.

## Proof:

To prove the completeness of truth tables, we need to show that for any well-formed formula, we can construct a truth table that exhaustively lists all possible combinations of truth values for its variables and evaluates the formula for each combination.

Let's consider a well-formed formula with n variables. We can construct a truth table with 2^n rows, where each row represents a unique combination of truth values for the variables.

For example, let's consider a well-formed formula with two variables, p and q. The truth table would have 2^2 = 4 rows:

| p | q | Formula |
|---|---|---------|
| T | T |         |
| T | F |         |
| F | T |         |
| F | F |         |

To evaluate the formula for each combination, we substitute the corresponding truth values into the formula and determine its truth value using the logical connectives and operators involved.

For example, let's say our formula is p ∧ q (logical AND). We substitute the truth values from each row into the formula:

- For the first row (p = T, q = T), we have: $T \land T$
- For the second row (p = T, q = F), we have: $T \land F$
- For the third row (p = F, q = T), we have: $F \land T$
- For the fourth row (p = F, q = F), we have: $F \land F$

We can now evaluate each of these expressions:

- $T \land T$ evaluates to T (True)
- $T \land F$ evaluates to F (False)
- $F \land T$ evaluates to F (False)
- $F \land F$ evaluates to F (False)

By evaluating the formula for each combination of truth values, we obtain the truth values for the entire truth table.

## Theorem: Consistency Test

A [[set]] of well-formed formulas is consistent if and only if there exists at least one row in their joint truth table where all formulas evaluate to true.

## Proof:

To prove the consistency test theorem, we need to show that a [[set]] of well-formed formulas is consistent if and only if there exists at least one row in their joint truth table where all formulas evaluate to true.

Let's consider a [[set]] of well-formed formulas {A_1, A_2, ..., A_n}. We can construct a joint truth table that includes all variables and formulas from the [[set]]. The joint truth table will have 2^m rows, where m is the total number of distinct variables in the [[set]].

For example, let's consider a [[set]] with two well-formed formulas: {p → q, ¬p ∨ r}. We can construct a joint truth table with 3 variables (p, q, r) and 2^3 = 8 rows:

| p | q | r | p → q | ¬p ∨ r |
|---|---|---|-------|--------|
| T | T | T |       |        |
| T | T | F |       |        |
| T | F | T |       |        |
| T | F | F |       |        |
| F | T | T |       |        |
| F | T | F |       |        |
| F | F | T |       |        |
| F | F | F |       |        |

To evaluate the formulas for each combination, we substitute the corresponding truth values into each formula and determine their truth values using the logical connectives and operators involved.

For example, let's evaluate the formulas p → q and ¬p ∨ r for each row:

- For the first row (p = T, q = T, r = T), we have: $T \rightarrow T$ and $\neg T \lor T$
- For the second row (p = T, q = T, r = F), we have: $T \rightarrow T$ and $\neg T \lor F$
- For the third row (p = T, q = F, r = T), we have: $T \rightarrow F$ and $\neg T \lor T$
- For the fourth row (p = T, q = F, r = F), we have: $T \rightarrow F$ and $\neg T \lor F$
- For the fifth row (p = F, q = T, r = T), we have: $F \rightarrow T$ and $\neg F \lor T$
- For the sixth row (p = F, q = T, r = F), we have: $F \rightarrow T$ and $\neg F \lor F$
- For the seventh row (p = F, q = F, r = T), we have: $F \rightarrow F$ and $\neg F \lor T$
- For the eighth row (p = F, q = F, r= 0), we have: $F \rightarrow 0$ and $\neg 0 \lor 0$

By evaluating each formula for every combination of truth values in their joint truth table, we can determine whether there exists at least one row where all formulas evaluate to true. If such a row exists, the [[set]] of formulas is consistent.

## Example: Consistency Test

Let's consider the [[set]] of well-formed formulas {p → q, ¬p ∨ r} and evaluate their consistency using a joint truth table.

| p | q | r | p → q | ¬p ∨ r |
|---|---|---|-------|--------|
| T | T | T |   T   |   T    |
| T | T | F |   T   |   F    |
| T | F | T |   F   |   T    |
| T | F | F |   F   |   F    |
| F | T | T |   T   |   T    |
| F | T | F |   T   |   F    |
| F 