#computing 
# Types of Proofs in [[Propositional Logic]]

In [[propositional logic]], various proof techniques are employed to establish the validity of logical arguments.

## 1. Vacuous Proof
   - Establishes the truth of a statement by demonstrating that its antecedent is false. 
   - If the condition required for the statement to be true never occurs, the statement itself is considered true.
### **Example:**  
- If $p$ is false in the [[implication]] $$(p \rightarrow q)$$, the statement is vacuously true regardless of the truth value of $q$.

## 2. Trivial Proof
   - Demonstrates the truth of a statement by directly showing its conclusion holds in all cases.
### Example:**  
- The statement $$(p \lor \neg p)$$ is always true, representing the principle of excluded middle.

## 3. Proof by Contrapositive
   - Establishes the validity of an [[implication]] by proving its contrapositive. 
   - If the contrapositive holds, then the original [[implication]] is also true.
### Example
- To prove $$(p \rightarrow q)$$ by contrapositive, assume $\neg q$ and deduce $\neg p$.

## 4. Direct Proof
   - begins with given premises and uses logical deductions to straightforwardly establish the truth of the conclusion.
   
## 5. Proof by Cases
   - dividing the problem into distinct scenarios or cases and proving each case separately. 
   
## 6. Proof by Mathematical Induction
   - used to establish statements about natural numbers or well-ordered sets.
   - typically involves proving a base case and then showing that if the statement holds for some value, it also holds for the next value, thereby demonstrating its validity for all values in the [[set]].
   
## 7. Proof by Contradiction
   - assumes the negation of the statement to be proved and derives a contradiction from it. 
   - By demonstrating that the negation leads to an inconsistency or impossibility, it establishes that the original statement must be true.

These proof techniques are fundamental in establishing the validity of arguments and mathematical theorems in [[propositional logic]].