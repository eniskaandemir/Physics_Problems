# Task 11 – Dynamics with a Time-Dependent Force

## Problem Statement

A particle of mass

$$
m = 3 \text{ kg}
$$

moves under the time-dependent force

$$
\vec{F}(t) = (15t,\; 3t - 12,\; -6t^2) \text{ N}
$$

Initial conditions are

$$
\vec{r}(0) = (5,2,-3) \text{ m}
$$

and

$$
\vec{v}(0) = (2,0,1) \text{ m/s}
$$

Determine the velocity and position as functions of time.

## Theory

Newton's second law gives

$$
\vec{F}(t) = m\vec{a}(t)
$$

Thus,

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

Velocity is obtained by integrating acceleration:

$$
\vec{v}(t) = \vec{v}(0) + \int_0^t \vec{a}(\tau)\,d\tau
$$

Position is obtained by integrating velocity:

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\,d\tau
$$

## Step-by-Step Solution

### 1. Acceleration

Since $m=3$ kg,

$$
\vec{a}(t) = \frac{1}{3}(15t,\; 3t - 12,\; -6t^2)
$$

Therefore,

$$
\vec{a}(t) = (5t,\; t - 4,\; -2t^2)
$$

### 2. Velocity

Integrate each component and apply the initial conditions.

#### x-component

$$
a_x = 5t
$$

Integrate:

$$
v_x(t) = \frac{5}{2}t^2 + C_x
$$

Use $v_x(0)=2$:

$$
C_x = 2
$$

So

$$
v_x(t) = \frac{5}{2}t^2 + 2
$$

#### y-component

$$
a_y = t - 4
$$

Integrate:

$$
v_y(t) = \frac{1}{2}t^2 - 4t + C_y
$$

Use $v_y(0)=0$:

$$
C_y = 0
$$

So

$$
v_y(t) = \frac{1}{2}t^2 - 4t
$$

#### z-component

$$
a_z = -2t^2
$$

Integrate:

$$
v_z(t) = -\frac{2}{3}t^3 + C_z
$$

Use $v_z(0)=1$:

$$
C_z = 1
$$

So

$$
v_z(t) = -\frac{2}{3}t^3 + 1
$$

Therefore,

$$
\vec{v}(t) = \left(\frac{5}{2}t^2 + 2,\; \frac{1}{2}t^2 - 4t,\; -\frac{2}{3}t^3 + 1\right)
$$

### 3. Position

Integrate the velocity components and apply the initial conditions.

#### x-component

$$
v_x(t) = \frac{5}{2}t^2 + 2
$$

Integrate:

$$
x(t) = \frac{5}{6}t^3 + 2t + C_1
$$

Use $x(0)=5$:

$$
C_1 = 5
$$

So

$$
x(t) = \frac{5}{6}t^3 + 2t + 5
$$

#### y-component

$$
v_y(t) = \frac{1}{2}t^2 - 4t
$$

Integrate:

$$
y(t) = \frac{1}{6}t^3 - 2t^2 + C_2
$$

Use $y(0)=2$:

$$
C_2 = 2
$$

So

$$
y(t) = \frac{1}{6}t^3 - 2t^2 + 2
$$

#### z-component

$$
v_z(t) = -\frac{2}{3}t^3 + 1
$$

Integrate:

$$
z(t) = -\frac{1}{6}t^4 + t + C_3
$$

Use $z(0)=-3$:

$$
C_3 = -3
$$

So

$$
z(t) = -\frac{1}{6}t^4 + t - 3
$$

Hence,

$$
\vec{r}(t) = \left(\frac{5}{6}t^3 + 2t + 5,\; \frac{1}{6}t^3 - 2t^2 + 2,\; -\frac{1}{6}t^4 + t - 3\right)
$$

## Final Result

Velocity:

$$
\vec{v}(t) = \left(\frac{5}{2}t^2 + 2,\; \frac{1}{2}t^2 - 4t,\; -\frac{2}{3}t^3 + 1\right)
$$

Position:

$$
\vec{r}(t) = \left(\frac{5}{6}t^3 + 2t + 5,\; \frac{1}{6}t^3 - 2t^2 + 2,\; -\frac{1}{6}t^4 + t - 3\right)
$$

## Interpretation

A time-dependent force produces a time-dependent acceleration, so neither the velocity nor the position follows a simple linear form. Each component evolves independently according to its own force component, and the full three-dimensional motion is obtained by integrating component by component.