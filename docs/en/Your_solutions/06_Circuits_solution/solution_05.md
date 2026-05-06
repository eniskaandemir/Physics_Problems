# Task 05 – Kirchhoff's Laws

## Problem Statement

Using Kirchhoff’s laws, determine the currents in the two-loop circuit shown.

Given:

$$ R_1 = 20\,\Omega $$

$$ R_2 = 10\,\Omega $$

$$ \mathcal{E}_1 = 4.5\,\text{V} $$

$$ \mathcal{E}_2 = 9.0\,\text{V} $$

Each source has internal resistance

$$ r_w = 1\,\Omega $$

## Theory

Kirchhoff’s current law states:

$$ \sum I_{\text{in}} = \sum I_{\text{out}} $$

Kirchhoff’s voltage law states:

$$ \sum \Delta V = 0 $$

Ohm’s law is:

$$ V = IR $$

## Step-by-Step Solution

### 1. Define Node Voltage

Let the top junction have potential

$$ V $$

Let the bottom junction be the reference point:

$$ V_B = 0 $$

Define currents from the top node to the bottom node.

### 2. Branch Currents

Middle branch current through $R_2$:

$$ I_2 = \frac{V}{10} $$

Left branch total resistance:

$$ R_{\text{left}} = 20 + 1 $$

$$ R_{\text{left}} = 21\,\Omega $$

Left branch current:

$$ I_1 = \frac{V - 4.5}{21} $$

Right branch current:

$$ I_3 = \frac{V - 9}{1} $$

$$ I_3 = V - 9 $$

### 3. Apply Kirchhoff’s Current Law

At the top node:

$$ I_1 + I_2 + I_3 = 0 $$

Substitute:

$$ \frac{V - 4.5}{21} + \frac{V}{10} + (V - 9) = 0 $$

Multiply by $210$:

$$ 10(V - 4.5) + 21V + 210(V - 9) = 0 $$

Expand:

$$ 10V - 45 + 21V + 210V - 1890 = 0 $$

$$ 241V - 1935 = 0 $$

$$ V = \frac{1935}{241} $$

$$ V \approx 8.03\,\text{V} $$

### 4. Calculate Currents

Left branch:

$$ I_1 = \frac{8.03 - 4.5}{21} $$

$$ I_1 \approx 0.168\,\text{A} $$

Middle branch:

$$ I_2 = \frac{8.03}{10} $$

$$ I_2 \approx 0.803\,\text{A} $$

Right branch:

$$ I_3 = 8.03 - 9 $$

$$ I_3 \approx -0.971\,\text{A} $$

## Final Result

$$ I_1 \approx 0.168\,\text{A} $$

$$ I_2 \approx 0.803\,\text{A} $$

$$ I_3 \approx -0.971\,\text{A} $$

The negative sign means the actual current in the right branch flows opposite to the assumed direction.

## Interpretation

The stronger $9$ V source drives current upward through the right branch. The negative value of $I_3$ indicates that the assumed current direction was opposite to the real direction.