#math #computing 

Sequent calculus is a formal system used in mathematical logic and proof theory to reason about logical formulas. It provides a framework for analyzing the validity of logical arguments and proofs. In this atomic note, we will explore the basics of sequent calculus, including its syntax, inference rules, and key theorems.

## Syntax

1. **Sequent Syntax**:
   - Sequents are expressions in the form Γ ⊢ Δ.
   - Γ and Δ are sets of formulas known as contexts.
   - The symbol ⊢ (turnstile) signifies "proves" or "entails".

2. **Contexts**:
   - Γ represents the [[set]] of formulas assumed true or known as premises.
   - Δ represents the [[set]] of formulas derived or concluded from premises.
   - Each context can contain zero or more formulas.
## Inference Rules

In sequent calculus, inference rules are used to derive new sequents from existing ones. Each rule specifies how certain patterns in a sequent can be transformed into new sequents. Let's discuss some commonly used inference rules:

### Identity Rule

The identity rule allows us to introduce or remove a formula from a context without affecting other formulas:

$$
\frac{}{\Gamma, A \vdash \Delta, A} \quad (\text{Identity})
$$

This rule states that if formula A is already present in both contexts Γ and Δ, we can add or remove it without changing anything else.

### Cut Rule

The cut rule allows us to split a proof into two separate parts by introducing an intermediate formula B:

$$
\frac{\Gamma \vdash \Delta, A \quad \Gamma', B \vdash \Delta'}{\Gamma, \Gamma' \vdash \Delta, B}  (\text{Cut})
$$

This rule states that if we have two separate proofs: one with premise A and conclusion Δ, and another with premise B and conclusion Δ', we can combine them by introducing the intermediate formula B.

### Structural Rules

The structural rules deal with the manipulation of contexts:

- Weakening Rule:

$$
\frac{\Gamma \vdash \Delta}{\Gamma, A \vdash \Delta} \quad (\text{Weakening Left})
$$

This rule allows us to add an arbitrary formula A to the left context Γ without affecting other formulas.

$$
\frac{\Gamma \vdash \Delta}{\Gamma \vdash \Delta, A}  \quad (\text{Weakening Right})
$$

Similarly, this rule allows us to add an arbitrary formula A to the right context Δ without affecting other formulas.

- Contraction Rule:

$$
\frac{\Gamma, A, A' \vdash \Delta}{\Gamma, A \vdash \Delta}  \quad (\text{Contraction Left})
$$

This rule allows us to remove duplicate occurrences of a formula in the left context Γ.

$$
\frac{\Gamma \vdash A, A', \Delta}{\Gamma \vdash A, \Delta}  \quad (\text{Contraction Right})
$$

Similarly, this rule allows us to remove duplicate occurrences of a formula in the right context Δ.

### [[Logical Rules]]

Sequent calculus also includes [[logical rules]] for various connectives such as conjunction (∧), disjunction (∨), [[implication]] (→), etc. These rules specify how these connectives behave in terms of sequents. Here are some examples:

- Conjunction Introduction Rule:

$$
\frac{\Gamma_1 \vdash A_1,\Delta_1  \quad  \Gamma_2 \vdash A_2,\Delta_2}{\Gamma_1,\Gamma_2 \vdash A_1 \land A_2,\Delta_1,\Delta_2}  \quad (\land I)
$$

This rule states that if we have two separate proofs with premises Γ1 and Γ2, and conclusions Δ1 and Δ2 respectively, we can combine them to prove the conjunction A1 ∧ A2.

- Disjunction Elimination Rule:

$$
\frac{\Gamma \vdash A \lor B,\Delta_1 \quad  \Gamma, A \vdash C,\Delta_2  \quad  \Gamma, B \vdash C,\Delta_3}{\Gamma \vdash C,\Delta_1,\Delta_2,\Delta_3}  \quad (\lor E)
$$

This rule states that if we have a proof of the disjunction A ∨ B and separate proofs for the implications A → C and B → C, then we can conclude C.

## Key Theorems

Sequent calculus provides a foundation for proving various logical theorems. Let's discuss a couple of key theorems:

### Cut Elimination Theorem

The Cut Elimination Theorem states that any sequent that can be proven using the cut rule can also be proven without using it. In other words, the cut rule is not essential for proving validity in sequent calculus.

### Soundness and Completeness

Sequent calculus is both sound and complete for classical [[propositional logic]]. Soundness means that if a sequent is provable, then it is logically valid. Completeness means that if a sequent is logically valid, then it is provable in sequent calculus.

These properties ensure that sequent calculus provides a reliable method for reasoning about logical formulas.

## Conclusion

Sequent calculus is a powerful formal system used in mathematical logic to reason about logical formulas. It consists of sequents with contexts representing premises and conclusions. Inference rules allow us to derive new sequents from existing ones, and various logical and structural rules provide the foundation for proving theorems. The Cut Elimination Theorem, soundness, and completeness are key results associated with sequent calculus.
