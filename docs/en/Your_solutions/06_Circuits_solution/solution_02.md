# Task 02 – Resistors

## Problem Statement

You have exactly three resistors, each with resistance

$$ R = 1\,\Omega $$

Determine all unique equivalent resistances that can be created using all three resistors.

## Theory

For series resistors:

$$ R_{\text{eq}} = R_1 + R_2 + R_3 $$

For parallel resistors:

$$ \frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} $$

## Step-by-Step Solution

### 1. All Three in Series

$$ R_{\text{eq}} = 1 + 1 + 1 $$

$$ R_{\text{eq}} = 3\,\Omega $$

### 2. All Three in Parallel

$$ \frac{1}{R_{\text{eq}}} = 1 + 1 + 1 $$

$$ \frac{1}{R_{\text{eq}}} = 3 $$

$$ R_{\text{eq}} = \frac{1}{3}\,\Omega $$

### 3. Two in Series, Then Parallel with the Third

First combine two resistors in series:

$$ R_s = 1 + 1 $$

$$ R_s = 2\,\Omega $$

Now place this in parallel with the third resistor:

$$ \frac{1}{R_{\text{eq}}} = \frac{1}{2} + 1 $$

$$ \frac{1}{R_{\text{eq}}} = \frac{3}{2} $$

$$ R_{\text{eq}} = \frac{2}{3}\,\Omega $$

### 4. Two in Parallel, Then Series with the Third

First combine two resistors in parallel:

$$ \frac{1}{R_p} = 1 + 1 $$

$$ R_p = \frac{1}{2}\,\Omega $$

Now add the third resistor in series:

$$ R_{\text{eq}} = 1 + \frac{1}{2} $$

$$ R_{\text{eq}} = \frac{3}{2}\,\Omega $$

## Final Result

The unique equivalent resistances are:

$$ R_{\text{eq}} = 3\,\Omega $$

$$ R_{\text{eq}} = \frac{3}{2}\,\Omega $$

$$ R_{\text{eq}} = \frac{2}{3}\,\Omega $$

$$ R_{\text{eq}} = \frac{1}{3}\,\Omega $$

## Interpretation

Series combinations increase resistance, while parallel combinations reduce resistance. Mixed arrangements produce intermediate values.