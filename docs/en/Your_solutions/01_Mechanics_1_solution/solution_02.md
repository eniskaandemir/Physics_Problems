# Task 02 – Range Optimization

## Problem Statement

Show analytically that the range

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

is maximized when

$$
\theta = 45^\circ
$$

---

## Theory

To maximize a function, take its derivative and set it equal to zero:

$$
\frac{dR}{d\theta} = 0
$$

---

## Step-by-Step Solution

Given:

$$
R(\theta) = \frac{v_0^2}{g} \sin(2\theta)
$$

Differentiate:

$$
\frac{dR}{d\theta} =
\frac{v_0^2}{g} \cdot 2\cos(2\theta)
$$

Set derivative equal to zero:

$$
2\cos(2\theta) = 0
$$

$$
\cos(2\theta) = 0
$$

Solve:

$$
2\theta = 90^\circ
$$

$$
\theta = 45^\circ
$$

---

### Second Derivative Test

$$
\frac{d^2R}{d\theta^2} =
-\frac{v_0^2}{g} \cdot 4\sin(2\theta)
$$

At $\theta = 45^\circ$:

$$
\sin(90^\circ) = 1
$$

$$
\frac{d^2R}{d\theta^2} < 0
$$

Thus, the point is a maximum.

---

## Final Result

$$
\theta = 45^\circ
$$

---

## Interpretation

The sine function reaches its maximum value at $90^\circ$.  
Since the range depends on $\sin(2\theta)$, the optimal launch angle is half of $90^\circ$, which is $45^\circ$.