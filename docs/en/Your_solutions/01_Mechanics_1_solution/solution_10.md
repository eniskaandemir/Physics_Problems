# Task 10 – Kinematics

## Problem Statement

Given:

$$
\vec{r}(t) = (a\cos(\omega t), b\sin(\omega t), bt)
$$

Find:

- trajectory
- path length
- interpretation

---

## Theory

Trajectory is obtained by eliminating $t$.

Arc length:

$$
s = \int |\vec{v}(t)| dt
$$

---

## Step-by-Step Solution

### 1. Trajectory

From components:

$$
x = a\cos(\omega t)
$$

$$
y = b\sin(\omega t)
$$

Thus:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

This is an ellipse.

---

### 2. Velocity

$$
\vec{v}(t) =
(-a\omega \sin(\omega t), b\omega \cos(\omega t), b)
$$

Magnitude:

$$
|\vec{v}| =
\sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}
$$

---

### 3. Path Length

$$
s = \int_0^{t_0} |\vec{v}(t)| dt
$$

No simple closed form unless special case.

---

## Final Result

Trajectory:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

---

## Interpretation

The motion is a **helical trajectory**:

- circular/elliptical in $xy$
- linear in $z$

Special case:

- if $a=b$ → circular helix