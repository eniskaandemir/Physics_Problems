# Task 06 – Kirchhoff's Laws Again

## Problem Statement

Determine the current flowing through the ammeter in the circuit shown.

Given:

$$ \mathcal{E}_1 = 9\,\text{V} $$

$$ \mathcal{E}_2 = 4.5\,\text{V} $$

$$ R_1 = 10\,\Omega $$

$$ R_2 = 20\,\Omega $$

Each source has internal resistance

$$ r_w = 1\,\Omega $$

## Theory

Kirchhoff’s current law states:

$$ \sum I_{\text{in}} = \sum I_{\text{out}} $$

Kirchhoff’s voltage law states:

$$ \sum \Delta V = 0 $$

A real voltage source can be modeled as an ideal source in series with internal resistance.

## Step-by-Step Solution

### 1. Define Node Voltages

Let the left node be the reference point:

$$ V_A = 0 $$

Let the upper-right node be:

$$ V_B $$

Let the lower-right node be:

$$ V_C $$

The ammeter is in the branch containing $R_2$, so the ammeter current is the current through $R_2$.

### 2. Ammeter Current

Current through $R_2$ from left to right is:

$$ I_A = \frac{V_A - V_B}{R_2} $$

Since $V_A = 0$:

$$ I_A = \frac{-V_B}{20} $$

### 3. Kirchhoff Equation at Node $B$

Using the branch relations from the diagram:

$$ (V_B + 4.5) + \frac{V_B}{20} + \frac{V_B - V_C}{10} = 0 $$

### 4. Kirchhoff Equation at Node $C$

$$ (V_C + 9) + \frac{V_C - V_B}{10} = 0 $$

### 5. Solve the System

The two equations are:

$$ (V_B + 4.5) + \frac{V_B}{20} + \frac{V_B - V_C}{10} = 0 $$

$$ (V_C + 9) + \frac{V_C - V_B}{10} = 0 $$

Solving gives:

$$ V_B \approx -4.66\,\text{V} $$

$$ V_C \approx -8.61\,\text{V} $$

### 6. Ammeter Current

$$ I_A = \frac{-V_B}{20} $$

$$ I_A = \frac{-(-4.66)}{20} $$

$$ I_A = \frac{4.66}{20} $$

$$ I_A \approx 0.233\,\text{A} $$

## Final Result

The current through the ammeter is:

$$ I_A \approx 0.233\,\text{A} $$

## Interpretation

The positive value means the current through the ammeter branch flows from left to right through $R_2$.