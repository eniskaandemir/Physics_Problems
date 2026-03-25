# Task 10 – Force Field and Power

## Problem Statement

A particle of mass

$$
m = 0.5 \text{ kg}
$$

moves according to

$$
x = 5t^2 - t, \qquad y = 2t^3, \qquad z = -3t + 2
$$

Determine the time dependence of:

1. velocity
2. momentum
3. acceleration
4. force
5. power transferred by the field

## Theory

For a position vector

$$
\vec{r}(t) = \big(x(t), y(t), z(t)\big)
$$

the velocity is

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

the acceleration is

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

the momentum is

$$
\vec{p}(t) = m\vec{v}(t)
$$

the force is

$$
\vec{F}(t) = m\vec{a}(t)
$$

and the instantaneous power is

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t)
$$

## Step-by-Step Solution

### 1. Position Vector

Write the motion in vector form:

$$
\vec{r}(t) = \big(5t^2 - t,\; 2t^3,\; -3t + 2\big)
$$

### 2. Velocity

Differentiate each component:

$$
\frac{dx}{dt} = 10t - 1
$$

$$
\frac{dy}{dt} = 6t^2
$$

$$
\frac{dz}{dt} = -3
$$

Thus,

$$
\vec{v}(t) = (10t - 1,\; 6t^2,\; -3)
$$

### 3. Momentum

Use

$$
\vec{p}(t) = m\vec{v}(t)
$$

with $m=0.5$ kg:

$$
\vec{p}(t) = 0.5(10t - 1,\; 6t^2,\; -3)
$$

Therefore,

$$
\vec{p}(t) = (5t - 0.5,\; 3t^2,\; -1.5)
$$

### 4. Acceleration

Differentiate the velocity:

$$
\frac{d}{dt}(10t - 1) = 10
$$

$$
\frac{d}{dt}(6t^2) = 12t
$$

$$
\frac{d}{dt}(-3) = 0
$$

Hence,

$$
\vec{a}(t) = (10,\; 12t,\; 0)
$$

### 5. Force

Use Newton's second law:

$$
\vec{F}(t) = m\vec{a}(t)
$$

$$
\vec{F}(t) = 0.5(10,\; 12t,\; 0)
$$

Thus,

$$
\vec{F}(t) = (5,\; 6t,\; 0)
$$

### 6. Power

Compute the dot product:

$$
P(t) = \vec{F}(t)\cdot\vec{v}(t)
$$

Substitute the expressions:

$$
P(t) = (5,\; 6t,\; 0)\cdot(10t - 1,\; 6t^2,\; -3)
$$

$$
P(t) = 5(10t - 1) + 6t(6t^2) + 0(-3)
$$

$$
P(t) = 50t - 5 + 36t^3
$$

Therefore,

$$
P(t) = 36t^3 + 50t - 5
$$

## Final Result

Velocity:

$$
\vec{v}(t) = (10t - 1,\; 6t^2,\; -3)
$$

Momentum:

$$
\vec{p}(t) = (5t - 0.5,\; 3t^2,\; -1.5)
$$

Acceleration:

$$
\vec{a}(t) = (10,\; 12t,\; 0)
$$

Force:

$$
\vec{F}(t) = (5,\; 6t,\; 0)
$$

Power:

$$
P(t) = 36t^3 + 50t - 5
$$

## Interpretation

The velocity and momentum change continuously because the motion is time-dependent in all coordinates. The force has a constant $x$-component and a time-dependent $y$-component. The power indicates how quickly the field transfers energy to the particle at each instant.