# Task 12 – Work and Energy with a Constant Force

## Problem Statement

A constant force acts on a body of mass

$$
m = 2 \text{ kg}
$$

The force is

$$
\vec{F} = [6, 2] \text{ N}
$$

The initial conditions are

$$
\vec{v}(0) = (1,-1) \text{ m/s}
$$

and

$$
\vec{r}(0) = (0,0) \text{ m}
$$

Determine:

1. $\vec{a}(t)$
2. $\vec{v}(t)$
3. $\vec{r}(t)$
4. the trajectory
5. the work done by the force at $t=3$ s
6. the consistency with the work-energy theorem

## Theory

For a constant force, acceleration is constant:

$$
\vec{a} = \frac{\vec{F}}{m}
$$

Velocity is found by integrating acceleration:

$$
\vec{v}(t) = \vec{v}_0 + \vec{a}t
$$

Position is then

$$
\vec{r}(t) = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2}\vec{a}t^2
$$

The work done by a constant force over displacement $\Delta \vec{r}$ is

$$
W = \vec{F} \cdot \Delta \vec{r}
$$

The work-energy theorem states

$$
W = \Delta K
$$

## Step-by-Step Solution

### 1. Acceleration

Given

$$
\vec{F} = (6,2)
$$

and

$$
m = 2
$$

the acceleration is

$$
\vec{a} = \frac{\vec{F}}{m} = \left(\frac{6}{2}, \frac{2}{2}\right)
$$

$$
\vec{a} = (3,1) \text{ m/s}^2
$$

Thus,

$$
\vec{a}(t) = (3,1)
$$

### 2. Velocity

Use

$$
\vec{v}(t) = \vec{v}_0 + \vec{a}t
$$

with

$$
\vec{v}_0 = (1,-1)
$$

Therefore,

$$
\vec{v}(t) = (1,-1) + (3,1)t
$$

So,

$$
\vec{v}(t) = (1+3t,\; -1+t)
$$

### 3. Position

Use

$$
\vec{r}(t) = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2}\vec{a}t^2
$$

Since $\vec{r}_0=(0,0)$,

$$
\vec{r}(t) = (1,-1)t + \frac{1}{2}(3,1)t^2
$$

Thus,

$$
\vec{r}(t) = \left(t + \frac{3}{2}t^2,\; -t + \frac{1}{2}t^2\right)
$$

So the coordinate equations are

$$
x(t) = t + \frac{3}{2}t^2
$$

$$
y(t) = -t + \frac{1}{2}t^2
$$

### 4. Trajectory

The motion is planar with parametric equations

$$
x(t) = t + \frac{3}{2}t^2
$$

and

$$
y(t) = -t + \frac{1}{2}t^2
$$

This trajectory is a parabola-like curve in the plane.

A simple Python script for plotting the trajectory is shown below.

```python
import numpy as np
import matplotlib.pyplot as plt

t = np.linspace(0, 3, 400)
x = t + 1.5 * t**2
y = -t + 0.5 * t**2

plt.figure()
plt.plot(x, y)
plt.xlabel("x")
plt.ylabel("y")
plt.title("Trajectory of the Body")
plt.grid(True)
plt.axis("equal")
plt.show()
```

### 5. Work Done by the Force at $t=3$ s

First compute the displacement from the origin to time $t=3$ s.

For $x(3)$:

$$
x(3) = 3 + \frac{3}{2}(9)
$$

$$
x(3) = 3 + 13.5 = 16.5
$$

For $y(3)$:

$$
y(3) = -3 + \frac{1}{2}(9)
$$

$$
y(3) = -3 + 4.5 = 1.5
$$

Thus,

$$
\Delta \vec{r} = (16.5, 1.5)
$$

Now compute the work:

$$
W = \vec{F}\cdot\Delta \vec{r}
$$

$$
W = (6,2)\cdot(16.5,1.5)
$$

$$
W = 6(16.5) + 2(1.5)
$$

$$
W = 99 + 3
$$

$$
W = 102 \text{ J}
$$

### 6. Check the Work-Energy Theorem

Initial kinetic energy:

$$
K_i = \frac{1}{2}m|\vec{v}(0)|^2
$$

Since

$$
\vec{v}(0) = (1,-1)
$$

we have

$$
|\vec{v}(0)|^2 = 1^2 + (-1)^2 = 2
$$

Thus,

$$
K_i = \frac{1}{2}(2)(2) = 2 \text{ J}
$$

Now compute the velocity at $t=3$:

$$
\vec{v}(3) = (1+9,\; -1+3) = (10,2)
$$

Then

$$
|\vec{v}(3)|^2 = 10^2 + 2^2 = 104
$$

So the final kinetic energy is

$$
K_f = \frac{1}{2}(2)(104) = 104 \text{ J}
$$

Hence,

$$
\Delta K = K_f - K_i
$$

$$
\Delta K = 104 - 2 = 102 \text{ J}
$$

This matches the work:

$$
W = \Delta K = 102 \text{ J}
$$

## Final Result

Acceleration:

$$
\vec{a}(t) = (3,1) \text{ m/s}^2
$$

Velocity:

$$
\vec{v}(t) = (1+3t,\; -1+t)
$$

Position:

$$
\vec{r}(t) = \left(t + \frac{3}{2}t^2,\; -t + \frac{1}{2}t^2\right)
$$

Work at $t=3$ s:

$$
W = 102 \text{ J}
$$

Work-energy theorem:

$$
W = \Delta K = 102 \text{ J}
$$

## Interpretation

A constant force produces constant acceleration, so the velocity changes linearly and the position changes quadratically with time. The equality between work and the change in kinetic energy confirms the work-energy theorem for this motion.