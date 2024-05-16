
The Routh [[Array]] is a tabular method used to determine the stability of a system by analyzing the coefficients of the characteristic equation. It was developed by Edward John Routh in the 19th century.

## Key Theorems and Definitions

1. **Routh-Hurwitz Criterion**: This criterion states that for a system to be stable, all the coefficients of the characteristic equation must be greater than zero.

2. **Routh [[Array]]**: The Routh [[Array]] is a table that helps in applying the Routh-Hurwitz criterion. It is constructed using the coefficients of the characteristic equation.

## Construction of Routh [[Array]]

To construct a Routh [[Array]] for a polynomial of degree n with coefficients $a_0, a_1, ..., a_n$, follow these steps:

1. Write down the coefficients in descending order.
2. Create the first two rows of the [[array]] using alternating coefficients.
3. Fill in the subsequent rows using these formulas:
   - For $i$th row and $j$th column: $$\text{Element}_{ij} = \frac{\text{Element}_{(i-1)j} \cdot \text{Element}_{(i-2)(j+1)} - \text{Element}_{(i-2)j} \cdot \text{Element}_{(i-1)(j+1)}}{\text{Element}_{(i-1)j}}$$
4. Count the number of sign changes in the first column to determine stability:
   - If there are no sign changes, all roots have negative real parts (system is stable).
   - If there are sign changes, count how many times they occur to determine unstable roots.

## Example

Given a characteristic equation $s^4 + 2s^3 + 3s^2 + 4s + 5 = 0$, construct its Routh [[Array]]:

|    |     |     |     |     |
|----|-----|-----|-----|-----|
| s^4| 1   | 3   | 5   |     |
| s^3| 2   | 4   |     |     |
| s^2|-7/2 |-5/6      |     |
| s^1|-11/6        |       |     |
| s^0|-17/12       |       |     |

In this example, since there are no sign changes in the first column, all roots have negative real parts and hence, the system is stable.

By following these steps and understanding how to interpret the results from a Routh [[Array]], one can effectively analyze and determine the stability of a given system using mathematical principles.