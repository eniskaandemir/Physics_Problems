# Task 02 – Electric Potential

## Problem Statement

Point charges

$$
+1 \text{ C}, \quad -2 \text{ C}, \quad +3 \text{ C}, \quad -4 \text{ C}
$$

are placed at the corners of a square of side length

$$
a = 1.0 \text{ m}
$$

in order.

Determine the electric potential at the center of the square.

## Theory

The electric potential produced by a point charge is

$$
V = k \frac{q}{r}
$$

The total electric potential from several charges is the algebraic sum:

$$
V_{\text{tot}} = \sum_i k \frac{q_i}{r_i}
$$

Electric potential is a scalar quantity, so signs are added directly.

## Step-by-Step Solution

### 1. Distance from the Center to a Corner

For a square of side length $a$, the distance from the center to each corner is

$$
r = \frac{a\sqrt{2}}{2}
$$

Since

$$
a = 1.0 \text{ m}
$$

we get

$$
r = \frac{\sqrt{2}}{2} \text{ m}
$$

### 2. Sum of Charges

Because all charges are at the same distance from the center, the potential can be written as

$$
V = \frac{k}{r}(q_1 + q_2 + q_3 + q_4)
$$

Now compute the total charge:

$$
q_1 + q_2 + q_3 + q_4 = 1 - 2 + 3 - 4
$$

$$
= -2 \text{ C}
$$

Thus,

$$
V = \frac{k}{r}(-2)
$$

### 3. Substitute Numerical Values

$$
V = \frac{8.99 \times 10^9 \cdot (-2)}{\sqrt{2}/2}
$$

Since

$$
\frac{1}{\sqrt{2}/2} = \frac{2}{\sqrt{2}} = \sqrt{2}
$$

we obtain

$$
V = -2 \sqrt{2} \cdot 8.99 \times 10^9
$$

$$
V \approx -2.54 \times 10^{10} \text{ V}
$$

## Final Result

The electric potential at the center is

$$
V \approx -2.54 \times 10^{10} \text{ V}
$$

## Interpretation

Because electric potential is a scalar, the individual contributions add directly. The negative charges dominate the sum, so the total potential at the center is negative.