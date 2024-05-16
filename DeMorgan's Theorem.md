#math
DeMorgan's Theorem is a fundamental concept in [[Boolean Algebra]] that describes the relationship between the logical operators "AND" and "OR" when negated. It provides a way to simplify complex logical expressions by transforming them into equivalent forms.

## Theorem Statement

DeMorgan's Theorem states that for any two logical variables or expressions, the negation of their conjunction (AND) is equivalent to the disjunction (OR) of their negations, and vice versa.

In mathematical notation, DeMorgan's Theorem can be stated as follows:

$$\neg (A \land B) \equiv \neg A \lor \neg B$$

$$\neg (A \lor B) \equiv \neg A \land \neg B$$

where $\neg$ represents the negation operator, $\land$ represents the conjunction operator (AND), and $\lor$ represents the disjunction operator (OR).

## Key Definitions

To fully understand DeMorgan's Theorem, it is important to be familiar with the following key definitions:

1. **Negation**: Negation is an operation that flips the truth value of a proposition. If $P$ is a proposition, then its negation $\neg P$ is true when $P$ is false, and false when $P$ is true.

2. **Conjunction**: Conjunction, denoted by $\land$, is an operation that combines two propositions and returns true only if both propositions are true; otherwise, it returns false.

3. **Disjunction**: Disjunction, denoted by $\lor$, is an operation that combines two propositions and returns true if at least one of the propositions is true; otherwise, it returns false.

## Example 1: Applying DeMorgan's Theorem

Let's consider an example to illustrate how DeMorgan's Theorem can be applied to simplify logical expressions.

Suppose we have the following logical expression:

$$\neg (P \land Q)$$

To apply DeMorgan's Theorem, we can use the first part of the theorem, which states that the negation of a conjunction is equivalent to the disjunction of their negations.

Using this, we can rewrite the expression as:

$$\neg P \lor \neg Q$$

Similarly, if we have the following expression:

$$\neg (P \lor Q)$$

We can apply the second part of DeMorgan's Theorem, which states that the negation of a disjunction is equivalent to the conjunction of their negations. Thus, we can rewrite it as:

$$\neg P \land \neg Q$$

These transformations allow us to simplify complex logical expressions and make them easier to analyze.

## Example 2: Applying DeMorgan's Theorem with Multiple Variables

DeMorgan's Theorem can also be applied when dealing with logical expressions involving multiple variables. Let's consider an example to illustrate this.

Suppose we have the following logical expression:

$$\neg (P \land (Q \lor R))$$

To simplify this expression using DeMorgan's Theorem, we start by applying the innermost operation first. We negate $Q \lor R$ using DeMorgan's Theorem for disjunctions:

$$\neg (P \land Q) \land (\neg Q \land \neg R)$$

Next, we negate $P \land Q$ using DeMorgan's Theorem for conjunctions:

$$(\neg P \lor \neg Q) \land (\neg Q \land \neg R)$$

Finally, we simplify further by distributing $\land$ over $\lor$:

$$(\neg P \land (\neg Q)) \lor (\neg P \land (\neg R))$$

This example demonstrates how DeMorgan's Theorem can be applied step-by-step to simplify complex logical expressions involving multiple variables.

## Conclusion

DeMorgan's Theorem is a powerful tool in [[Boolean Algebra]] that allows us to simplify logical expressions by transforming them into equivalent forms. By understanding the relationships between negation, conjunction, and disjunction, we can apply DeMorgan's Theorem to simplify complex expressions and analyze their properties more easily.