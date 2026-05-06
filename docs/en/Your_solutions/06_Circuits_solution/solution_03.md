# Task 03 – Mixed Circuit 01

## Problem Statement

Calculate the equivalent resistance of the circuit shown in the figure.

All resistors have resistance

$$ R = 5\,\Omega $$

## Theory

For series resistors:

$$ R_{\text{eq}} = R_1 + R_2 + \cdots $$

For parallel resistors:

$$ \frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots $$

## Step-by-Step Solution

### 1. Upper-Left Branch

The left vertical resistor and top horizontal resistor are in series:

$$ R_A = 5 + 5 $$

$$ R_A = 10\,\Omega $$

### 2. Middle Branch

The middle path contains three resistors in series:

$$ R_B = 5 + 5 + 5 $$

$$ R_B = 15\,\Omega $$

The upper-left branch and middle branch form one path:

$$ R_{AB} = 10 + 15 $$

$$ R_{AB} = 25\,\Omega $$

### 3. Right Branch

The right side contains two resistors in series:

$$ R_C = 5 + 5 $$

$$ R_C = 10\,\Omega $$

### 4. Parallel Combination

The two main branches are in parallel:

$$ \frac{1}{R_P} = \frac{1}{25} + \frac{1}{10} $$

$$ \frac{1}{R_P} = \frac{2}{50} + \frac{5}{50} $$

$$ \frac{1}{R_P} = \frac{7}{50} $$

$$ R_P = \frac{50}{7}\,\Omega $$

$$ R_P \approx 7.14\,\Omega $$

### 5. Add Bottom Series Resistor

The bottom resistor is in series with the parallel network:

$$ R_{\text{eq}} = R_P + 5 $$

$$ R_{\text{eq}} = \frac{50}{7} + 5 $$

$$ R_{\text{eq}} = \frac{50}{7} + \frac{35}{7} $$

$$ R_{\text{eq}} = \frac{85}{7}\,\Omega $$

$$ R_{\text{eq}} \approx 12.14\,\Omega $$

## Final Result

$$ R_{\text{eq}} = \frac{85}{7}\,\Omega $$

$$ R_{\text{eq}} \approx 12.14\,\Omega $$

## Interpretation

The circuit contains both series and parallel sections. The parallel part reduces the total resistance, while the bottom resistor increases it because it is in series.