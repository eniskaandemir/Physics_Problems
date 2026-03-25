# Task 03 – Conservation of Energy

## Problem Statement

A pendulum of length $1.0$ m is released from an initial angle of $15^\circ$.

Determine the speed of the pendulum bob at the bottom of the swing.

## Theory

For an ideal pendulum with no dissipative forces, mechanical energy is conserved.

At release:

- kinetic energy is zero
- gravitational potential energy is maximum

At the bottom:

- potential energy is minimum
- kinetic energy is maximum

Thus,

$$
mgh = \frac{1}{2}mv^2
$$

The vertical height drop from angle $\theta$ to the lowest point is

$$
h = L(1-\cos\theta)
$$

## Step-by-Step Solution

### 1. Determine the Height Drop

The pendulum length is

$$
L = 1.0 \text{ m}
$$

The initial angle is

$$
\theta = 15^\circ
$$

Use

$$
h = L(1-\cos\theta)
$$

Substitute the values:

$$
h = 1.0(1-\cos 15^\circ)
$$

Using

$$
\cos 15^\circ \approx 0.9659
$$

we get

$$
h = 1.0(1 - 0.9659)
$$

$$
h \approx 0.0341 \text{ m}
$$

### 2. Apply Conservation of Energy

At the top,

$$
E_i = mgh
$$

At the bottom,

$$
E_f = \frac{1}{2}mv^2
$$

Set them equal:

$$
mgh = \frac{1}{2}mv^2
$$

Cancel the mass:

$$
gh = \frac{1}{2}v^2
$$

Multiply by $2$:

$$
2gh = v^2
$$

Take the square root:

$$
v = \sqrt{2gh}
$$

Substitute $g = 9.81 \text{ m/s}^2$ and $h = 0.0341$ m:

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

$$
v \approx \sqrt{0.669}
$$

$$
v \approx 0.818 \text{ m/s}
$$

## Final Result

The speed of the pendulum bob at the bottom is

$$
v \approx 0.82 \text{ m/s}
$$

## Interpretation

The initial gravitational potential energy is converted into kinetic energy as the bob descends. Since the release angle is small, the height drop is modest, so the final speed is also relatively small.