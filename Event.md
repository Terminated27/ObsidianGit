#math #stats 

In statistics, an **event** refers to a specific outcome or [[set]] of outcomes of an experiment or random phenomenon. Events are fundamental building blocks in probability theory and are used to describe the likelihood of certain outcomes occurring.

## Definitions

1. **[[Sample Space]] ($\Omega$)**: The [[sample space]] is the [[set]] of all possible outcomes of an experiment. It is denoted by $\Omega$. For example, when flipping a fair coin, the [[sample space]] is $\Omega = \{H, T\}$ where $H$ represents heads and $T$ represents tails.

2. **Event ($A$)**: An event is a [[subset]] of the [[sample space]], representing a collection of outcomes that we are interested in. It is denoted by $A$. For example, if we define event $A$ as getting heads when flipping a fair coin, then $A = \{H\}$.

3. **Empty [[Set]] ($\emptyset$)**: The empty [[set]] represents an event with no possible outcomes. It is denoted by $\emptyset$. For example, if we define event $B$ as getting a 7 when rolling a standard six-sided die, then $B = \emptyset$ since there are no possible outcomes that satisfy this condition.

4. **Complement of an Event ($A^c$)**: The complement of an event $A$, denoted by $A^c$, consists of all outcomes in the [[sample space]] that are not part of event $A$. In other words, it represents all outcomes that do not satisfy the condition specified by event $A$. For example, if we define event $C$ as getting tails when flipping a fair coin, then $C = \{T\}$ and its complement is given by $C^c = \{H\}$.

## Properties

1. **Union**: The union of two events $A$ and $B$, denoted by $A \cup B$, represents the event that either $A$ or $B$ (or both) occur. It consists of all outcomes that are in either $A$ or $B$. Mathematically, $A \cup B = \{x : x \in A \text{ or } x \in B\}$.

2. **Intersection**: The intersection of two events $A$ and $B$, denoted by $A \cap B$, represents the event that both $A$ and $B$ occur simultaneously. It consists of all outcomes that are in both $A$ and $B$. Mathematically, $A \cap B = \{x : x \in A \text{ and } x \in B\}$.

3. **Mutually Exclusive (Disjoint) Events**: Two events are said to be mutually exclusive if they cannot occur at the same time, i.e., their intersection is empty ($A \cap B = \emptyset$). For example, when rolling a standard six-sided die, the events "getting an odd number" and "getting an even number" are mutually exclusive.

## Example

Consider an experiment of rolling a fair six-sided die. Let's define the following events:

- Event A: Getting an even number.
- Event B: Getting a number less than 4.
- Event C: Getting a prime number.

We can determine these events as follows:

- Event A: $\{2, 4, 6\}$
- Event B: $\{1, 2, 3\}$
- Event C: $\{2, 3, 5\}$

Now let's explore some properties of these events:

1. Union of Events A and B: 
   - Event A $\cup$ Event B = $\{1, 2, 3, 4, 6\}$ (Getting an even number or a number less than 4)

2. Intersection of Events B and C: 
   - Event B $\cap$ Event C = $\{2\}$ (Getting a number less than 4 and a prime number)

3. Complement of Event A: 
   - Event A$^c$ = $\{1, 3, 5\}$ (Not getting an even number)

These properties and definitions help us analyze and calculate probabilities of various events in probability theory.

## Theorems

1. **De Morgan's Laws**: De Morgan's Laws provide a way to express the complement of unions and intersections of events.
   - Complement of Union: $(A \cup B)^c = A^c \cap B^c$
   - Complement of Intersection: $(A \cap B)^c = A^c \cup B^c$

2. **Inclusion-Exclusion Principle**: The inclusion-exclusion principle is used to calculate the probability of the union of multiple events.
   - $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
   - For three events: $P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(A \cap C) - P(B \cap C) + P(A \cap B \cap C)$

These theorems provide useful tools for calculating probabilities involving multiple events.

By understanding the concepts and properties related to events in statistics, we can analyze experiments and random phenomena more effectively, making informed decisions based on probability calculations.