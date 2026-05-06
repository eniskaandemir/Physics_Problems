# Task 01 – Series and Parallel Circuit

## Problem Statement

Three resistors are given:

$$
R_1 = 15\,\Omega
$$

$$
R_2 = 30\,\Omega
$$

$$
R_3 = 50\,\Omega
$$

The battery voltage is

$$
V = 12\,\text{V}
$$

Determine:

1. the equivalent resistance when the resistors are connected in series
2. the current supplied by the battery in the series case
3. the equivalent resistance when the resistors are connected in parallel
4. the current supplied by the battery in the parallel case

## Theory

### Series Connection

For resistors in series:

$$
R_{\text{eq}} = R_1 + R_2 + R_3
$$

The same current flows through all resistors.

Using Ohm’s law:

$$
I = \frac{V}{R}
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
\frac{1}{R_3}
$$

In parallel circuits, the voltage across each resistor is the same.

## Step-by-Step Solution

### 1. Series Equivalent Resistance

Add the resistances:

$$
R_{\text{series}}
=
15 + 30 + 50
$$

$$
R_{\text{series}} = 95\,\Omega
$$

### 2. Current in the Series Circuit

Use Ohm’s law:

$$
I_{\text{series}}
=
\frac{V}{R_{\text{series}}}
$$

Substitute values:

$$
I_{\text{series}}
=
\frac{12}{95}
$$

$$
I_{\text{series}}
\approx 0.126\,\text{A}
$$

### 3. Parallel Equivalent Resistance

Use the parallel formula:

$$
\frac{1}{R_{\text{parallel}}}
=
\frac{1}{15}
+
\frac{1}{30}
+
\frac{1}{50}
$$

Find a common denominator:

$$
\frac{1}{15}
=
0.0667
$$

$$
\frac{1}{30}
=
0.0333
$$

$$
\frac{1}{50}
=
0.0200
$$

Add:

$$
\frac{1}{R_{\text{parallel}}}
=
0.0667 + 0.0333 + 0.0200
$$

$$
\frac{1}{R_{\text{parallel}}}
=
0.1200
$$

Thus,

$$
R_{\text{parallel}}
=
\frac{1}{0.1200}
$$

$$
R_{\text{parallel}}
\approx 8.33\,\Omega
$$

### 4. Current in the Parallel Circuit

Apply Ohm’s law:

$$
I_{\text{parallel}}
=
\frac{12}{8.33}
$$

$$
I_{\text{parallel}}
\approx 1.44\,\text{A}
$$

## Final Result

### Series Circuit

Equivalent resistance:

$$
R_{\text{series}} = 95\,\Omega
$$

Battery current:

$$
I_{\text{series}} \approx 0.126\,\text{A}
$$

### Parallel Circuit

Equivalent resistance:

$$
R_{\text{parallel}} \approx 8.33\,\Omega
$$

Battery current:

$$
I_{\text{parallel}} \approx 1.44\,\text{A}
$$

## Interpretation

In a series connection, resistances add directly, producing a larger equivalent resistance and therefore a smaller current.

In a parallel connection, the equivalent resistance becomes smaller than any individual resistor, allowing much larger current to flow from the battery.