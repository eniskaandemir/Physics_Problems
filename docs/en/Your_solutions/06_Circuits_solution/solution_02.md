# Task 02 – Resistors

## Problem Statement

You have exactly three resistors, each with resistance

$$
R = 1\,\Omega
$$

Determine all unique equivalent resistances that can be formed using all three resistors.

## Theory

Resistors may be connected:

- entirely in series
- entirely in parallel
- in mixed series-parallel combinations

### Series Formula

$$
R_{\text{eq}} = R_1 + R_2 + \cdots
$$

### Parallel Formula

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

### 1. All Three in Series

$$
R_{\text{eq}} = 1 + 1 + 1
$$

$$
R_{\text{eq}} = 3\,\Omega
$$

### 2. All Three in Parallel

$$
\frac{1}{R_{\text{eq}}}
=
1 + 1 + 1
$$

$$
\frac{1}{R_{\text{eq}}} = 3
$$

$$
R_{\text{eq}} = \frac{1}{3}\,\Omega
$$

### 3. Two in Series, Then Parallel with the Third

First combine two resistors in series:

$$
R_s = 1 + 1 = 2\,\Omega
$$

Now place this in parallel with the remaining resistor:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{2}
+
1
$$

$$
\frac{1}{R_{\text{eq}}}
=
\frac{3}{2}
$$

$$
R_{\text{eq}}
=
\frac{2}{3}\,\Omega
$$

### 4. Two in Parallel, Then Series with the Third

First combine two resistors in parallel:

$$
\frac{1}{R_p}
=
1 + 1
$$

$$
R_p = \frac{1}{2}\,\Omega
$$

Now add the third resistor in series:

$$
R_{\text{eq}}
=
1 + \frac{1}{2}
$$

$$
R_{\text{eq}}
=
\frac{3}{2}\,\Omega
$$

## Final Result

The unique equivalent resistances are:

$$
3\,\Omega
$$

$$
\frac{3}{2}\,\Omega
$$

$$
\frac{2}{3}\,\Omega
$$

$$
\frac{1}{3}\,\Omega
$$

## Interpretation

By combining identical resistors in different configurations, both larger and smaller equivalent resistances can be produced. Series connections increase resistance, while parallel connections reduce it.