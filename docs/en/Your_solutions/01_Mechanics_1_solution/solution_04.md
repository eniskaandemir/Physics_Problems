# Task 04 – Vector Calculus

## Problem Statement

The position vector is given by

$$
\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}
$$

Find:

- velocity vector
- acceleration vector

---

## Theory

Velocity is the first derivative of position:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

Acceleration is the second derivative:

$$
\vec{a}(t) = \frac{d^2\vec{r}}{dt^2}
$$

---

## Step-by-Step Solution

### 1. Velocity

Differentiate each component:

$$
\vec{v}(t) =
\frac{d}{dt}(3t^2)\hat{i} + \frac{d}{dt}(5t - 8t^2)\hat{j}
$$

$$
\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

---

### 2. Acceleration

Differentiate again:

$$
\vec{a}(t) =
\frac{d}{dt}(6t)\hat{i} + \frac{d}{dt}(5 - 16t)\hat{j}
$$

$$
\vec{a}(t) = (6)\hat{i} + (-16)\hat{j}
$$

---

## Final Result

Velocity:

$$
\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

Acceleration:

$$
\vec{a}(t) = 6\hat{i} - 16\hat{j}
$$

---

## Interpretation

The acceleration is constant, meaning the motion is uniformly accelerated.  
The velocity changes linearly with time due to constant acceleration.