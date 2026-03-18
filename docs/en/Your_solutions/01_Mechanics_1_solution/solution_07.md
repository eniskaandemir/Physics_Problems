# Task 07 – Parametric Motion and Acceleration

## Problem Statement

Given:

$$
x(t) = 2t^2, \qquad y(t) = 3t^3
$$

Determine:

- eliminate parameter $t$
- trajectory equation
- velocity and acceleration
- whether acceleration is constant

---

## Theory

Velocity:

$$
\vec{v}(t) = \left(\frac{dx}{dt}, \frac{dy}{dt}\right)
$$

Acceleration:

$$
\vec{a}(t) = \left(\frac{d^2x}{dt^2}, \frac{d^2y}{dt^2}\right)
$$

---

## Step-by-Step Solution

### 1. Eliminate Parameter

From

$$
x = 2t^2
$$

$$
t = \sqrt{\frac{x}{2}}
$$

Substitute into $y$:

$$
y = 3t^3 = 3\left(\frac{x}{2}\right)^{3/2}
$$

---

### 2. Velocity

$$
v_x = \frac{dx}{dt} = 4t
$$

$$
v_y = \frac{dy}{dt} = 9t^2
$$

Thus:

$$
\vec{v}(t) = (4t, 9t^2)
$$

Magnitude:

$$
|\vec{v}| = \sqrt{(4t)^2 + (9t^2)^2}
$$

$$
|\vec{v}| = \sqrt{16t^2 + 81t^4}
$$

---

### 3. Acceleration

$$
a_x = 4
$$

$$
a_y = 18t
$$

Thus:

$$
\vec{a}(t) = (4, 18t)
$$

Magnitude:

$$
|\vec{a}| = \sqrt{16 + 324t^2}
$$

---

## Final Result

Trajectory:

$$
y = 3\left(\frac{x}{2}\right)^{3/2}
$$

Velocity:

$$
\vec{v}(t) = (4t, 9t^2)
$$

Acceleration:

$$
\vec{a}(t) = (4, 18t)
$$

---

## Interpretation

The acceleration is **not constant** because its vertical component depends on time.  
The trajectory is a nonlinear curve.