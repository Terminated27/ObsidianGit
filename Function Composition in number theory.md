

# Function Composition

Function composition is a fundamental concept in mathematics where two functions are combined to create a new function. Given two functions $f: A \rightarrow B$ and $g: B \rightarrow C$, the composition of $f$ and $g$, denoted as $g \circ f$, is defined as:

$$ (g \circ f)(x) = g(f(x)) $$

In other words, the output of function $f$ is used as the input for function $g$. 

## Key Theorems

### Associativity of Function Composition
Function composition is associative, meaning that for any functions $f: A \rightarrow B$, $g: B \rightarrow C$, and $h: C \rightarrow D$, the following holds:

$$ h \circ (g \circ f) = (h \circ g) \circ f $$

### Identity Function
For any [[set]] $A$ and function $f: A \rightarrow A$, the identity function $\text{id}_A: A \rightarrow A$ defined by $\text{id}_A(x) = x$ for all $x\in A$ serves as the identity element with respect to function composition:

$$ f \circ \text{id}_A = f = \text{id}_A \circ f $$

## Examples

**Example 1:** Let $f(x) = x^2$ and $g(x) = 2x + 1$. Find $(g \circ f)(x)$.

**Solution:** 
First, we find $(g\circ f)(x)$ by substituting the expression for $f(x)$ into $g(x)$:
$$ (g\circ f)(x) = g(f(x)) = g(x^2) = 2x^2 + 1 $$

**Example 2:** Let $h(x) = e^{2x}$ and $k(x) = x^3$. Find $(k\circ h)(x)$.

**Solution:** 
Similarly, we find $(k\circ h)(x)$ by substituting the expression for $h(x)$ into k(x):
$$ (k\circ h)(x) = k(h(x))= k(e^{2x})= (e^{2x})^3= e^{6x} $$

Function composition allows us to combine functions in a meaningful way, providing a powerful tool in mathematical analysis and problem-solving.



# Function Composition in Number Theory

In number theory, function composition refers to the operation of applying one function to the output of another function. This concept is particularly important when dealing with functions that operate on integers or other discrete mathematical objects.

## Definition

Given two functions $f: A \rightarrow B$ and $g: B \rightarrow C$, the composition of $f$ and $g$, denoted by $g \circ f$, is defined as:

$$(g \circ f)(x) = g(f(x))$$

where $x \in A$.

## Theorems

### Theorem 1: Associativity of Function Composition
For functions $f: A \rightarrow B$, $g: B \rightarrow C$, and $h: C \rightarrow D$, the composition of functions is associative, meaning $(h \circ g) \circ f = h \circ (g \circ f)$.

### Theorem 2: Identity Function
For any [[set]] $A$ and function $f: A \rightarrow A$, the identity function $\text{id}_A : A \rightarrow A$ defined by $\text{id}_A(x) = x$ for all $x\in A$ serves as the identity element for function composition, i.e., $\text{id}_A \circ f = f = f\circ\text{id}_A$.

## Example

Let's consider two functions in number theory:

$f(x) = x^2$

$g(x) = 2x + 1$

We can find the composition $(g\circ f)(x)$ as follows:

$(g\circ f)(x) = g(f(x))$

$(g\circ f)(x) = g(x^2)$

$(g\circ f)(x) = 2(x^2) + 1$

Therefore, $(g\circ f)(x) = 2x^2 + 1$.