# Task 06 – Variable Velocity

## Problem Statement

The velocity of an object is given by

$v(t) = t^2 + 2t - 5$

Given that

$x(0) = 4$

Find:

- the position at $t=3$
- the acceleration at $t=3$

---

## Theory

Velocity is the derivative of position:

$$
v(t) = \frac{dx}{dt}
$$

Thus, position is obtained by integration:

$$
x(t) = \int v(t)\,dt
$$

Acceleration is the derivative of velocity:

$$
a(t) = \frac{dv}{dt}
$$

---

## Step-by-Step Solution

### 1. Position Function

Integrate velocity:

$$
x(t) = \int (t^2 + 2t - 5)\,dt
$$

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + C
$$

---

### 2. Determine Constant

Using initial condition:

$$
x(0) = 4
$$

$$
4 = 0 + 0 - 0 + C
$$

$$
C = 4
$$

Thus:

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + 4
$$

---

### 3. Position at $t=3$

$$
x(3) = \frac{27}{3} + 9 - 15 + 4
$$

$$
x(3) = 9 + 9 - 15 + 4
$$

$$
x(3) = 7
$$

---

### 4. Acceleration

Differentiate velocity:

$$
a(t) = 2t + 2
$$

$$
a(3) = 6 + 2 = 8
$$

---

## Final Result

Position:

$$
x(3) = 7
$$

Acceleration:

$$
a(3) = 8
$$

---

## Interpretation

The object's motion is non-uniform since velocity is time-dependent.  
Acceleration increases linearly with time.