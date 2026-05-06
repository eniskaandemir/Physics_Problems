# Task 04 – Mixed Circuit 02

## Problem Statement

Calculate the equivalent resistance of the circuit shown in the figure.

All resistors have resistance

$$ R = 10\,\Omega $$

## Theory

For series resistors:

$$ R_{\text{eq}} = R_1 + R_2 + \cdots $$

For parallel resistors:

$$ \frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots $$

## Step-by-Step Solution

### 1. Top Branch

The top branch contains two resistors in series:

$$ R_{\text{top}} = 10 + 10 $$

$$ R_{\text{top}} = 20\,\Omega $$

### 2. Bottom Branch

The lower branch begins with one resistor in series with two parallel resistors.

First combine the two parallel resistors:

$$ \frac{1}{R_p} = \frac{1}{10} + \frac{1}{10} $$

$$ \frac{1}{R_p} = \frac{2}{10} $$

$$ R_p = 5\,\Omega $$

Now add the first bottom resistor:

$$ R_{\text{bottom}} = 10 + 5 $$

$$ R_{\text{bottom}} = 15\,\Omega $$

### 3. Parallel Combination of Top and Bottom Branches

$$ \frac{1}{R_{\text{inside}}} = \frac{1}{20} + \frac{1}{15} $$

$$ \frac{1}{R_{\text{inside}}} = \frac{3}{60} + \frac{4}{60} $$

$$ \frac{1}{R_{\text{inside}}} = \frac{7}{60} $$

$$ R_{\text{inside}} = \frac{60}{7}\,\Omega $$

$$ R_{\text{inside}} \approx 8.57\,\Omega $$

### 4. Add Final Series Resistor

The resistor on the far right is in series with the inner network:

$$ R_{\text{eq}} = R_{\text{inside}} + 10 $$

$$ R_{\text{eq}} = \frac{60}{7} + 10 $$

$$ R_{\text{eq}} = \frac{60}{7} + \frac{70}{7} $$

$$ R_{\text{eq}} = \frac{130}{7}\,\Omega $$

$$ R_{\text{eq}} \approx 18.57\,\Omega $$

## Final Result

$$ R_{\text{eq}} = \frac{130}{7}\,\Omega $$

$$ R_{\text{eq}} \approx 18.57\,\Omega $$

## Interpretation

The internal network is reduced by combining parallel branches, then the final right resistor is added in series.