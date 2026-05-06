# Task 15 – Resistor Cube

## Problem Statement

A cube is formed from 12 identical resistors, each with resistance

$$
R
$$

Determine the equivalent resistance between two opposite corners of the cube.

## Theory

The cube possesses strong geometric symmetry.

When a voltage is applied between opposite corners:

- equivalent nodes have the same potential
- symmetric branches carry equal currents

This symmetry allows the circuit to be reduced to simpler parallel-series combinations.

## Step-by-Step Solution

### 1. Symmetry Argument

Choose opposite corners:

- one corner at potential $V$
- opposite corner at potential $0$

The three vertices adjacent to the first corner are equivalent by symmetry.

Similarly, the three vertices adjacent to the opposite corner are also equivalent.

Thus the cube reduces to three stages:

1. three resistors in parallel
2. six resistors in the middle
3. three resistors in parallel

### 2. First Group

Three equal resistors in parallel:

$$
R_1
=
\frac{R}{3}
$$

### 3. Middle Group

The middle section becomes six equal resistors arranged symmetrically.

Its equivalent resistance is

$$
R_2
=
\frac{R}{6}
$$

### 4. Final Group

Again:

$$
R_3
=
\frac{R}{3}
$$

### 5. Total Resistance

All three equivalent sections are in series:

$$
R_{\text{eq}}
=
\frac{R}{3}
+
\frac{R}{6}
+
\frac{R}{3}
$$

Find a common denominator:

$$
R_{\text{eq}}
=
\frac{2R}{6}
+
\frac{R}{6}
+
\frac{2R}{6}
$$

$$
R_{\text{eq}}
=
\frac{5R}{6}
$$

However, because the middle reduction double-counts equivalent branches, the correct cube reduction yields

$$
R_{\text{eq}}
=
\frac{5}{6}R
$$

between adjacent corners, while for opposite corners the standard result is

$$
R_{\text{eq}}
=
\frac{5}{6}R
$$

Wait — for opposite corners of a cube, the exact equivalent resistance is

$$
R_{\text{eq}}
=
\frac{5}{6}R
$$

## Final Result

The equivalent resistance between opposite corners of the cube is

$$
R_{\text{eq}}
=
\frac{5}{6}R
$$

## Interpretation

The high symmetry of the cube causes current to split equally among equivalent branches. This allows a seemingly complicated three-dimensional resistor network to be reduced to a simple equivalent resistance.