# Task 15 – Resistor Cube

## Problem Statement

A cube is constructed from $12$ identical resistors, one on each edge.

Each resistor has resistance:

$$ R $$

Determine the equivalent resistance between two opposite corners of the cube.

## Theory

The cube has strong symmetry. When a voltage is applied between two opposite corners:

- the three vertices adjacent to the first corner have equal potential
- the three vertices adjacent to the opposite corner have equal potential
- equal-potential nodes can be joined without changing the circuit

This reduces the cube to a simpler series-parallel network.

## Step-by-Step Solution

### 1. First Group

From the first corner, current splits equally into three identical resistors.

These three resistors are in parallel:

$$ R_1 = \frac{R}{3} $$

### 2. Middle Group

Between the two sets of equal-potential nodes, there are six identical resistors in parallel.

Thus:

$$ R_2 = \frac{R}{6} $$

### 3. Final Group

Near the opposite corner, current recombines through three identical resistors in parallel:

$$ R_3 = \frac{R}{3} $$

### 4. Total Resistance

The three reduced sections are in series:

$$ R_{\text{eq}} = R_1 + R_2 + R_3 $$

$$ R_{\text{eq}} = \frac{R}{3} + \frac{R}{6} + \frac{R}{3} $$

Use common denominator $6$:

$$ R_{\text{eq}} = \frac{2R}{6} + \frac{R}{6} + \frac{2R}{6} $$

$$ R_{\text{eq}} = \frac{5R}{6} $$

## Final Result

$$ R_{\text{eq}} = \frac{5R}{6} $$

## Interpretation

The cube can be simplified using symmetry. Equal-potential vertices allow the network to reduce to three series sections: three parallel resistors, six parallel resistors, and three parallel resistors.