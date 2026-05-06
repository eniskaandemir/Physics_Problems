# Task 04 – Mixed Circuit 02

## Problem Statement

Determine the equivalent resistance of the circuit shown in the figure.

All resistors have resistance

$$
R = 10\,\Omega
$$

## Theory

The circuit can be simplified by identifying series and parallel sections.

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

### 1. Identify the Top Branch

The top branch contains two resistors in series.

Each resistor has resistance

$$
10\,\Omega
$$

Therefore,

$$
R_{\text{top}} = 10 + 10
$$

$$
R_{\text{top}} = 20\,\Omega
$$

### 2. Identify the Lower Branch

The lower branch begins with one resistor in series.

After that, the circuit splits into two parallel resistors.

First, combine the two parallel resistors:

$$
\frac{1}{R_p}
=
\frac{1}{10}
+
\frac{1}{10}
$$

$$
\frac{1}{R_p}
=
\frac{2}{10}
$$

$$
R_p = 5\,\Omega
$$

Now add the first lower resistor in series:

$$
R_{\text{bottom}} = 10 + 5
$$

$$
R_{\text{bottom}} = 15\,\Omega
$$

### 3. Combine Top and Bottom Branches

The top branch and lower branch are connected in parallel between the same two nodes.

Thus,

$$
\frac{1}{R_{\text{inside}}}
=
\frac{1}{R_{\text{top}}}
+
\frac{1}{R_{\text{bottom}}}
$$

Substitute:

$$
\frac{1}{R_{\text{inside}}}
=
\frac{1}{20}
+
\frac{1}{15}
$$

Find a common denominator:

$$
\frac{1}{R_{\text{inside}}}
=
\frac{3}{60}
+
\frac{4}{60}
$$

$$
\frac{1}{R_{\text{inside}}}
=
\frac{7}{60}
$$

Therefore,

$$
R_{\text{inside}} = \frac{60}{7}\,\Omega
$$

$$
R_{\text{inside}} \approx 8.57\,\Omega
$$

### 4. Add the Final Series Resistor

The resistor on the far right is in series with the whole inner network.

Therefore,

$$
R_{\text{eq}}
=
R_{\text{inside}} + 10
$$

$$
R_{\text{eq}}
=
\frac{60}{7} + 10
$$

Convert to a common denominator:

$$
R_{\text{eq}}
=
\frac{60}{7}
+
\frac{70}{7}
$$

$$
R_{\text{eq}}
=
\frac{130}{7}\,\Omega
$$

Numerically,

$$
R_{\text{eq}}
\approx 18.57\,\Omega
$$

## Final Result

The equivalent resistance is

$$
R_{\text{eq}}
=
\frac{130}{7}\,\Omega
$$

or approximately

$$
R_{\text{eq}}
\approx 18.57\,\Omega
$$

## Interpretation

The circuit contains both series and parallel combinations. The top branch has a larger resistance than the lower branch, so more current would flow through the lower branch. The final resistor on the right increases the total resistance because it is in series with the entire network.