# Task 05 – Kirchhoff's Laws

## Problem Statement

Using Kirchhoff’s laws, determine the currents in the two-loop circuit shown in the figure.

Given:

$$
R_1 = 20\,\Omega
$$

$$
R_2 = 10\,\Omega
$$

$$
\mathcal{E}_1 = 4.5\,\text{V}
$$

$$
\mathcal{E}_2 = 9.0\,\text{V}
$$

Each source has internal resistance

$$
r_w = 1\,\Omega
$$

The goal is to find the currents through the main branches of the circuit.

## Theory

Kirchhoff’s laws are:

### Kirchhoff’s Current Law

At any junction, the total current entering equals the total current leaving.

$$
\sum I_{\text{in}} = \sum I_{\text{out}}
$$

### Kirchhoff’s Voltage Law

Around any closed loop, the sum of potential rises and drops is zero.

$$
\sum \Delta V = 0
$$

Ohm’s law relates voltage and current:

$$
V = IR
$$

## Step-by-Step Solution

### 1. Define Nodes and Current Directions

Let the top junction have potential

$$
V
$$

and let the bottom junction be the reference point:

$$
V_B = 0
$$

Define currents from the top node to the bottom node.

The middle branch current is through $R_2$:

$$
I_2 = \frac{V}{10}
$$

The left branch contains $R_1$, the internal resistance of $\mathcal{E}_1$, and the source $\mathcal{E}_1$.

The total resistance in the left branch is

$$
R_{\text{left}} = 20 + 1 = 21\,\Omega
$$

Using the polarity shown in the diagram, the left branch current is

$$
I_1 = \frac{V - 4.5}{21}
$$

The right branch contains the internal resistance and the $9$ V source:

$$
I_3 = \frac{V - 9}{1}
$$

### 2. Apply Kirchhoff’s Current Law

At the top node, the algebraic sum of currents leaving the node is zero:

$$
I_1 + I_2 + I_3 = 0
$$

Substitute the branch expressions:

$$
\frac{V - 4.5}{21} + \frac{V}{10} + (V - 9) = 0
$$

### 3. Solve for the Node Voltage

Multiply through by $210$:

$$
10(V - 4.5) + 21V + 210(V - 9) = 0
$$

Expand:

$$
10V - 45 + 21V + 210V - 1890 = 0
$$

Combine terms:

$$
241V - 1935 = 0
$$

Solve for $V$:

$$
241V = 1935
$$

$$
V = \frac{1935}{241}
$$

$$
V \approx 8.03\,\text{V}
$$

### 4. Calculate the Currents

For the left branch:

$$
I_1 = \frac{V - 4.5}{21}
$$

$$
I_1 = \frac{8.03 - 4.5}{21}
$$

$$
I_1 \approx 0.168\,\text{A}
$$

For the middle branch:

$$
I_2 = \frac{V}{10}
$$

$$
I_2 = \frac{8.03}{10}
$$

$$
I_2 \approx 0.803\,\text{A}
$$

For the right branch:

$$
I_3 = V - 9
$$

$$
I_3 = 8.03 - 9
$$

$$
I_3 \approx -0.971\,\text{A}
$$

The negative sign means that the actual current in the right branch flows opposite to the assumed direction.

## Final Result

With currents initially assumed from the top node to the bottom node:

$$
I_1 \approx 0.168\,\text{A}
$$

$$
I_2 \approx 0.803\,\text{A}
$$

$$
I_3 \approx -0.971\,\text{A}
$$

Therefore, the actual right-branch current has magnitude

$$
|I_3| \approx 0.971\,\text{A}
$$

and flows from the bottom node to the top node.

## Interpretation

The stronger $9$ V source drives current upward through the right branch. Part of this current flows down through the middle resistor $R_2$, and the rest flows through the left branch. The negative sign in $I_3$ is not an error; it only indicates that the original assumed current direction was opposite to the physical current direction.