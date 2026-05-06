# Task 03 – Mixed Circuit 01

## Problem Statement

Determine the equivalent resistance of the circuit shown in the figure.

All resistors have resistance

$$
R = 5\,\Omega
$$

## Theory

To determine the equivalent resistance:

1. identify series connections
2. identify parallel branches
3. simplify the circuit step-by-step
4. combine the reduced sections

### Series Connection

For resistors in series:

$$
R_{\text{eq}} = R_1 + R_2 + \cdots
$$

### Parallel Connection

For resistors in parallel:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{R_1}
+
\frac{1}{R_2}
+
\cdots
$$

## Step-by-Step Solution

### 1. Identify the Main Branches

The circuit contains three branches between the left and right terminals.

#### Upper-left branch

This branch contains:

- left vertical resistor
- top horizontal resistor

These two resistors are in series:

$$
R_A = 5 + 5
$$

$$
R_A = 10\,\Omega
$$

#### Middle branch

The middle branch contains:

- two vertical resistors
- one lower horizontal resistor

All are in series:

$$
R_B = 5 + 5 + 5
$$

$$
R_B = 15\,\Omega
$$

The upper-left branch and middle branch connect in series through the same path:

$$
R_{AB} = 10 + 15
$$

$$
R_{AB} = 25\,\Omega
$$

### 2. Right Branch

The right branch contains two vertical resistors in series:

$$
R_C = 5 + 5
$$

$$
R_C = 10\,\Omega
$$

### 3. Parallel Combination

The two large branches are connected in parallel:

- branch 1:

$$
25\,\Omega
$$

- branch 2:

$$
10\,\Omega
$$

Use the parallel formula:

$$
\frac{1}{R_P}
=
\frac{1}{25}
+
\frac{1}{10}
$$

Find common denominator:

$$
\frac{1}{R_P}
=
\frac{2}{50}
+
\frac{5}{50}
$$

$$
\frac{1}{R_P}
=
\frac{7}{50}
$$

Therefore:

$$
R_P
=
\frac{50}{7}\,\Omega
$$

$$
R_P
\approx 7.14\,\Omega
$$

### 4. Bottom Resistor

The bottom resistor is connected in series with the entire parallel network.

Thus:

$$
R_{\text{eq}}
=
R_P + 5
$$

$$
R_{\text{eq}}
=
\frac{50}{7} + 5
$$

Convert to common denominator:

$$
R_{\text{eq}}
=
\frac{50}{7}
+
\frac{35}{7}
$$

$$
R_{\text{eq}}
=
\frac{85}{7}\,\Omega
$$

$$
R_{\text{eq}}
\approx 12.14\,\Omega
$$

## Final Result

The equivalent resistance of the circuit is

$$
R_{\text{eq}}
=
\frac{85}{7}\,\Omega
$$

or approximately

$$
R_{\text{eq}}
\approx 12.14\,\Omega
$$

## Interpretation

The circuit combines both series and parallel resistor arrangements.

- series sections increase resistance
- parallel branches reduce resistance

The final equivalent resistance is therefore smaller than the total sum of all resistors but larger than the smallest branch resistance.