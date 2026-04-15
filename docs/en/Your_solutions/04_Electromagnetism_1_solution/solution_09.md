# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with velocity

$$
\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \text{ m/s}
$$

in a magnetic field

$$
\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \text{ T}
$$

Determine the magnitude of the magnetic force on the proton.

## Theory

The magnetic force on a moving charge is

$$
\vec{F} = q \vec{v} \times \vec{B}
$$

For a proton,

$$
q = e = 1.60 \times 10^{-19} \text{ C}
$$

The magnitude is

$$
F = q |\vec{v} \times \vec{B}|
$$

## Step-by-Step Solution

### 1. Compute the Cross Product

Write the determinant:

$$
\vec{v} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{vmatrix}
$$

Expand:

$$
\vec{v} \times \vec{B}
=
\hat{i}[(-4)(-1) - (1)(2)]
-
\hat{j}[(2)(-1) - (1)(1)]
+
\hat{k}[(2)(2) - (-4)(1)]
$$

$$
=
\hat{i}(4 - 2)
-
\hat{j}(-2 - 1)
+
\hat{k}(4 + 4)
$$

$$
=
2\hat{i} + 3\hat{j} + 8\hat{k}
$$

### 2. Compute Its Magnitude

$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2}
$$

$$
= \sqrt{4 + 9 + 64}
$$

$$
= \sqrt{77}
$$

### 3. Multiply by the Proton Charge

$$
F = q \sqrt{77}
$$

$$
F = (1.60 \times 10^{-19})\sqrt{77}
$$

Since

$$
\sqrt{77} \approx 8.775
$$

we get

$$
F \approx 1.40 \times 10^{-18} \text{ N}
$$

## Final Result

The magnitude of the magnetic force is

$$
F \approx 1.4 \times 10^{-18} \text{ N}
$$

## Interpretation

The magnetic force depends only on the component of velocity perpendicular to the field. The cross product automatically captures this directional dependence and produces a force perpendicular to both $\vec{v}$ and $\vec{B}$.