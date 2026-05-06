# Task 06 – Kirchhoff's Laws Again

## Problem Statement

Determine the current flowing through the ammeter in the circuit shown.

From the figure:

$$
\mathcal{E}_1 = 9\,\text{V}
$$

$$
\mathcal{E}_2 = 4.5\,\text{V}
$$

$$
R_1 = 10\,\Omega
$$

$$
R_2 = 20\,\Omega
$$

Each source has internal resistance

$$
r_w = 1\,\Omega
$$

## Theory

Kirchhoff's laws are used to analyze circuits with multiple loops.

### Kirchhoff's Current Law

At a junction:

$$
\sum I_{\text{in}} = \sum I_{\text{out}}
$$

### Kirchhoff's Voltage Law

Around a closed loop:

$$
\sum \Delta V = 0
$$

A source with internal resistance can be treated as an ideal voltage source in series with a resistor.

## Step-by-Step Solution

### 1. Define Nodes

Let the left node be the reference point:

$$
V_A = 0
$$

Let the upper-right node be

$$
V_B
$$

and the lower-right node be

$$
V_C
$$

The ammeter is in the branch containing $R_2$, so the ammeter current is the current through $R_2$.

### 2. Current Through the $R_2$ Branch

The current through $R_2$ from left to right is

$$
I_A = \frac{V_A - V_B}{R_2}
$$

Since

$$
V_A = 0
$$

this becomes

$$
I_A = \frac{-V_B}{20}
$$

### 3. Apply Kirchhoff's Current Law at Node $B$

At node $B$, currents through the top source branch, through $R_2$, and through $R_1$ must balance.

Using the polarities shown in the diagram:

$$
(V_B + 4.5) + \frac{V_B}{20} + \frac{V_B - V_C}{10} = 0
$$

### 4. Apply Kirchhoff's Current Law at Node $C$

At node $C$, currents through the bottom source branch and through $R_1$ must balance:

$$
(V_C + 9) + \frac{V_C - V_B}{10} = 0
$$

### 5. Solve the System

The system is

$$
(V_B + 4.5) + \frac{V_B}{20} + \frac{V_B - V_C}{10} = 0
$$

$$
(V_C + 9) + \frac{V_C - V_B}{10} = 0
$$

Solving gives

$$
V_B \approx -4.66\,\text{V}
$$

and

$$
V_C \approx -8.61\,\text{V}
$$

### 6. Calculate the Ammeter Current

The ammeter current is

$$
I_A = \frac{-V_B}{20}
$$

Substitute:

$$
I_A = \frac{-(-4.66)}{20}
$$

$$
I_A = \frac{4.66}{20}
$$

$$
I_A \approx 0.233\,\text{A}
$$

## Final Result

The current through the ammeter is approximately

$$
I_A \approx 0.233\,\text{A}
$$

## Interpretation

The positive value means that the current through the ammeter branch flows from the left side of the circuit toward the right side through $R_2$. The two voltage sources oppose each other through different branches, so Kirchhoff's laws are needed to determine the actual current distribution.