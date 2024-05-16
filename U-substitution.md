#math #calculus 
simple example and provide atomic notes for u-substitution. We'll use the [[integral]] $$\int 2xe^{x^2}dx$$ as our example.

**Example:** Evaluate $\int 2xe^{x^2}dx$.

**Step 1: Identify a Complex Part**

- The complex part is $xe^{x^2}dx$ in the integrand.

**Step 2: Choose u**

- Choose $u=x^2$ as a suitable substitution.

**Step 3: Calculate du**

- Find du by differentiating u with respect to x: $du=2xdx$

**Step 4: Rewrite the [[Integral]]**

- Rewrite the [[integral]] using u: $\int e^u du$.

**Step 5: Simplify**

- The [[integral]] is now simpler: $\int e^u du$.

**Step 6: Integrate with Respect to u**

- Integrate the simpler [[integral]] with respect to u: 11��+�=��+�11​eu+C=eu+C.

**Step 7: Back-substitute**

- Replace �u with the original expression involving �x: ��2+�ex2+C.

**Step 8: No Need to Adjust Limits**

- No need to adjust the limits of [[integration]] for indefinite integrals.

**Step 9: Evaluate**

- The result is ��2+�ex2+C.

**Step 10: Check Completeness**

- Verify that the result matches the original [[integral]]'s value: ∫2���2 ��=��2+�∫2xex2dx=ex2+C.

**General Formula for u-substitution:**

- Given an [[integral]] ∫�(�(�))�′(�) ��∫f(g(x))g′(x)dx, perform u-substitution as follows:
    1. Choose �=�(�)u=g(x).
    2. Calculate ��=�′(�) ��du=g′(x)dx.
    3. Rewrite the [[integral]] in terms of �u: ∫�(�) ��∫f(u)du.
    4. Simplify and integrate with respect to �u.
    5. Back-substitute to express the result in terms of the original variable.
    6. Check completeness to ensure the result matches the original [[integral]].