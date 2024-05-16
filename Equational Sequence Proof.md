#math #computing 
In [[propositional logic]], an equational sequence proof is a method used to derive logical equivalences between propositional formulas. It involves a series of steps, each of which is justified by applying certain rules of inference or known logical equivalences. This note will provide an overview of the key concepts and techniques involved in equational sequence proofs.

## Definitions

Before diving into the proof technique, let's define some important terms:

1. **[[Propositional Logic]]**: A branch of logic that deals with propositions (statements that are either true or false) and their logical connectives (such as AND, OR, NOT).
2. **Logical Equivalence**: Two propositional formulas are said to be logically equivalent if they have the same truth value for every possible assignment of truth values to their variables.
3. **[[Sequent]]**: A [[sequent]] is an expression of the form Γ ⊢ Δ, where Γ and Δ are sets of propositional formulas. It represents a claim that if all formulas in Γ are true, then at least one formula in Δ must also be true.
4. **Equational Sequence Proof**: A proof technique used to establish logical equivalence between two propositional formulas by deriving a series of sequents.

## Key Theorems

In equational sequence proofs, we often make use of several key theorems related to logical equivalences. Here are some important ones:
$\bot$ = Not true
$\top$ = true

1. **Identity Laws**:
   - $P \land \top \equiv P$ (AND Identity)
   - $P \lor \bot \equiv P$ (OR Identity)

2. **Domination Laws**:
   - $P \lor \top \equiv \top$ (OR Domination)
   - $P \land \bot \equiv \bot$ (AND Domination)

3. **Idempotent Laws**:
   - $P \lor P \equiv P$ (OR Idempotence)
   - $P \land P \equiv P$ (AND Idempotence)

4. **Double Negation Law**:
   - $\neg(\neg P) \equiv P$

5. **De Morgan's Laws**:
   - $\neg(P \land Q) \equiv (\neg P) \lor (\neg Q)$ (AND De Morgan)
   - $\neg(P \lor Q) \equiv (\neg P) \land (\neg Q)$ (OR De Morgan)

6. **Distributive Laws**:
   - $P \land (Q \lor R) \equiv (P \land Q) \lor (P \land R)$ (AND over OR)
   - $P \lor (Q \land R) \equiv (P \lor Q) \land (P \lor R)$ (OR over AND)
   
 7.  **Definition of [[Implication]]**:
   - $P \rightarrow Q \equiv \neg P \lor Q$. 

8. **Absorption Law**:
   - $P \lor (P \land Q) \equiv P$ (OR Absorption)
   - $P \land (P \lor Q) \equiv P$ (AND Absorption)
   
1. **[[Biconditional]] Definition**:
   - $P \leftrightarrow Q \equiv (P \rightarrow Q) \land (Q \rightarrow P)$ 
   - $P \leftrightarrow \neg Q \equiv (P \rightarrow \neg Q) \land (\neg Q \rightarrow P)$
## Example of Equational Sequence Proof

Let's demonstrate an equational sequence proof 

Given the [[sequent]]: $P \land (Q \lor R) \vdash (P \lor Q) \land (P \lor R)$

1. **Apply the distributive law (AND over OR):**
   - $P \land (Q \lor R) \vdash (P \land Q) \lor (P \land R)$

2. **Apply the distributive law (OR over AND):**
   - $P \land (Q \lor R) \vdash (P \lor P) \land (P \lor R)$

3. **Apply the idempotent law (OR):**
   - $P \land (Q \lor R) \vdash P \land (P \lor R)$

4. **Apply absorption law:**
   - $P \land (Q \lor R) \vdash P$

Through these steps, we've successfully derived the logical equivalence $P \land (Q \lor R) \equiv P$. This example illustrates how equational sequence proofs proceed through a series of steps, applying various [[logical rules]] and equivalences to establish the desired result.
