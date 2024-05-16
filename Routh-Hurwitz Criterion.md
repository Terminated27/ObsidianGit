
The Routh-Hurwitz Criterion is a method used to determine the stability of a linear time-invariant system by examining the coefficients of the characteristic equation. It provides a necessary and sufficient condition for stability based on the locations of the roots of the characteristic equation in the left half-plane.

## Key Theorems

1. **[[Routh's Stability Criterion]]**: For a polynomial with real coefficients $a_n, a_{n-1}, ..., a_0$, all roots of the polynomial have negative real parts if and only if all the determinants in the first column of the [[Routh array]] are positive.

2. **[[Hurwitz's Stability Criterion]]**: For a polynomial with real coefficients $a_n, a_{n-1}, ..., a_0$, all roots of the polynomial have negative real parts if and only if all leading principal minors of the Hurwitz matrix are positive.

## Definitions

- **Characteristic Equation**: The characteristic equation of a linear time-invariant system is given by $$
    \Delta(s) = s^n + a_{n-1}s^{n-1} + \cdots + a_1s + a_0
$$ where $a_i$ are coefficients.

- **[[Routh Array]]**: The [[Routh array]] is constructed using the coefficients of the characteristic equation to determine stability.

## Step-by-step Example

Consider a second-order system with characteristic equation $$
    \Delta(s) = s^2 + 4s + 4
$$

### Step 1: Constructing [[Routh Array]]

|   |   |
|---|---|
| s^2 | 1 |
| s^1 | 4 |
| s^0 | 4 |

### Step 2: Completing [[Routh Array]]

|     |     |
| --- | --- |
| s^2 | 1   |
| s^1 | 4   |
| s^0 | 4   |

For this example, since all elements in the first column are positive, we can conclude that both roots have negative real parts, indicating stability.

By using the Routh-Hurwitz Criterion, engineers can quickly assess system stability without explicitly calculating roots.