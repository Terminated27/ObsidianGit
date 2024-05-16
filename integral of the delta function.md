#Conttime 

1. **Sifting Property with Unit [[Step Function]]:**
   
   The sifting property with the unit [[step function]] is given by:
   
   $$\int_{-\infty}^{\infty} \delta(x - a) u(x) dx = u(a)$$
   
   This property states that the [[integral]] of the product of the [[Dirac delta function]] and the unit [[step function]] is equal to the value of the unit [[step function]] at the point where the delta function is located.

2. **Scaling Property with Unit [[Step Function]]:**
   
   The scaling property with the unit [[step function]] is given by:
   
   $$\int_{-\infty}^{\infty} A\delta(x) u(x) dx = A \cdot u(0) = A$$
   
   This property states that scaling the [[Dirac delta function]] by a factor A and convolving it with the unit [[step function]] simply scales the unit [[step function]] by the same factor A.

3. **Symmetry Property with Unit [[Step Function]]:**
   
   The symmetry property with the unit [[step function]] states that:
   
   $$u(-x) = 1 - u(x)$$
   
   This property arises because the unit [[step function]] is 0 for $$x < 0$$ and 1 for $$x \geq 0$$

4. **Shifting Property with Unit [[Step Function]]:**
   
   If $\delta(x)$ is shifted by an amount c, it becomes $\delta(x - c)$:
   
   $$\int_{-\infty}^{\infty} \delta(x - c) u(x) dx = u(c)$$
   
   This property states that shifting the [[Dirac delta function]] by an amount c and convolving it with the unit [[step function]] gives the value of the unit [[step function]] at the point c.

5. **Linearity Property with Unit [[Step Function]]:**
   
   The linearity property with the unit [[step function]] states that:
   
   $$\int_{-\infty}^{\infty} [a\delta(x) + b\delta(x - c)] u(x) dx = a \cdot u(0) + b \cdot u(c) = a + b \cdot u(c)$$
   
   This property holds for linear combinations of Dirac delta functions convolved with the unit [[step function]].

6. **[[Derivative]] Property with Unit [[Step Function]]:**
   
   The [[derivative]] property with the unit [[step function]] is given by:
   
   $$\int_{-\infty}^{\infty} f(x) \delta'(x - a) u(x) dx = -f'(a) \cdot u(a)$$
   
   This property allows differentiation of the [[Dirac delta function]] under the [[integral]] sign when convolved with the unit [[step function]] and a sufficiently smooth function $$f(x)$$.