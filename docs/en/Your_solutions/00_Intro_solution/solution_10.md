# Task 10 – Infinite Series

## Problem Statement

An ant starts at the origin and moves according to the pattern:

- $1 \text{ m}$ east
- $\frac{1}{2} \text{ m}$ north
- $\frac{1}{3} \text{ m}$ west
- $\frac{1}{4} \text{ m}$ south
- $\frac{1}{5} \text{ m}$ east

and so on.

Determine the final position of the ant.

## Theory

The motion alternates between horizontal and vertical directions:

- odd-numbered steps in the horizontal direction
- even-numbered steps in the vertical direction

The horizontal displacement is an alternating series:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots
$$

The vertical displacement is also an alternating series:

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
$$

These are standard infinite series.

The Leibniz series gives

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \frac{\pi}{4}
$$

Also,

$$
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \ln 2
$$

From this, the even-term alternating series can be derived.

## Step-by-Step Solution

### Horizontal Displacement

The ant moves horizontally on odd-numbered steps:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots
$$

This is the Leibniz series for arctangent:

$$
x = \frac{\pi}{4}
$$

### Vertical Displacement

The vertical motion is

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
$$

Factor out $\frac{1}{2}$:

$$
y = \frac{1}{2}\left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots \right)
$$

The expression in parentheses is the alternating harmonic series:

$$
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \ln 2
$$

Therefore,

$$
y = \frac{1}{2}\ln 2
$$

### Final Coordinate

The ant starts at the origin, so its final position is

$$
\left(\frac{\pi}{4}, \frac{1}{2}\ln 2\right)
$$

## Final Result

The final position of the ant is

$$
\left(\frac{\pi}{4}, \frac{1}{2}\ln 2\right)
$$

## Interpretation

The horizontal and vertical displacements both converge because the step lengths form alternating series with decreasing magnitudes. Even though the ant makes infinitely many moves, the total displacement approaches a finite point in the plane.