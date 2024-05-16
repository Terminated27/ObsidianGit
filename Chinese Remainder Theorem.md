#computing 

The Chinese Remainder Theorem is a fundamental result in number theory that provides a solution to a system of simultaneous congruences. It states that if $n_1, n_2, \ldots, n_k$ are [[pairwise coprime integers]], then for any integers $a_1, a_2, \ldots, a_k$, the system of congruences:

$$
\begin{align*}
x &\equiv a_1 \pmod{n_1} \\
x &\equiv a_2 \pmod{n_2} \\
&\vdots \\
x &\equiv a_k \pmod{n_k}
\end{align*}
$$

has a unique solution [[modulo]] $N = n_1n_2\ldots n_k$.

## Key Theorems and Definitions

### The Chinese Remainder Theorem (CRT)

Given $n_1, n_2, \ldots, n_k$ pairwise [[coprime]] integers and $a_1, a_2, \ldots, a_k$ any integers, the system of congruences has a unique solution [[modulo]] $N = n_1n_2\ldots n_k$.

### Corollary of CRT

If $n_i$ are pairwise [[coprime]] and $\gcd(n_i,n) = 1$ for all $i$, then the system of congruences:

$$
\begin{align*}
x &\equiv a_i \pmod{n_i} \\
x &\equiv b \pmod{n}
\end{align*}
$$

has a unique solution [[modulo]] $N = n n_1n_2\ldots n_k$.

## Step-by-Step Example

Consider the following system of congruences:

$$
\begin{align*}
x &\equiv 2 \pmod{3} \\
x &\equiv 3 \pmod{5} \\
x &\equiv 2 \pmod{7}
\end{align*}
$$

We can apply the Chinese Remainder Theorem to find the unique solution. First, calculate $N = 3 \times 5 \times 7 = 105$. Then find the modular inverses:

- For $105/3=35$, the modular inverse is $35^{-1} \equiv 2 \pmod{3}$.
- For $105/5=21$, the modular inverse is $21^{-1} \equiv 1 \pmod{5}$.
- For $105/7=15$, the modular inverse is $15^{-1} \equiv 1 \pmod{7}$.

Finally, compute the solution:

$$
x = (2\times35\times2 + 3\times21\times3 + 2\times15\times2) \%105 = 23
$$

Therefore, the unique solution to the system of congruences is $x \equiv 23 (\text{mod }105)$.