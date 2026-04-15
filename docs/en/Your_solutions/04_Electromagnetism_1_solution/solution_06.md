# Task 06 – Field from a System of Charges

## Problem Statement

Two point charges are placed on the $x$-axis:

- $+q$ at $(-a,0)$
- $+2q$ at $(a,0)$

Determine:

1. the electric field $\vec{E}(0,y)$, $\vec{E}(x,0)$, and in general $\vec{E}(x,y)$
2. the conditions for $E_x = 0$, $E_y = 0$, and $\vec{E}=0$
3. the field for

$$
a = 0.2 \text{ m}, \quad y = 0.3 \text{ m}, \quad q = 2\,\mu\text{C}
$$

4. the limit $y \gg a$

## Theory

The electric field of a point charge $Q$ at position $\vec{r}_0$ is

$$
\vec{E}(\vec{r}) = kQ \frac{\vec{r}-\vec{r}_0}{|\vec{r}-\vec{r}_0|^3}
$$

The total field is the vector sum of the fields from both charges.

## Step-by-Step Solution

### 1. General Field $\vec{E}(x,y)$

For the charge $+q$ at $(-a,0)$:

$$
\vec{r} - \vec{r}_1 = (x+a, y)
$$

So

$$
\vec{E}_1 = kq \frac{(x+a)\hat{i} + y\hat{j}}{\left[(x+a)^2 + y^2\right]^{3/2}}
$$

For the charge $+2q$ at $(a,0)$:

$$
\vec{r} - \vec{r}_2 = (x-a, y)
$$

Thus

$$
\vec{E}_2 = 2kq \frac{(x-a)\hat{i} + y\hat{j}}{\left[(x-a)^2 + y^2\right]^{3/2}}
$$

Hence the total field is

$$
\vec{E}(x,y) =
kq \frac{(x+a)\hat{i} + y\hat{j}}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{(x-a)\hat{i} + y\hat{j}}{\left[(x-a)^2 + y^2\right]^{3/2}}
$$

### 2. Field on the $y$-Axis: $\vec{E}(0,y)$

Set $x=0$:

$$
\vec{E}(0,y) =
kq \frac{a\hat{i} + y\hat{j}}{(a^2+y^2)^{3/2}}
+
2kq \frac{-a\hat{i} + y\hat{j}}{(a^2+y^2)^{3/2}}
$$

Combine terms:

$$
\vec{E}(0,y) =
\frac{kq}{(a^2+y^2)^{3/2}}
\left[
(a-2a)\hat{i} + (y+2y)\hat{j}
\right]
$$

$$
\vec{E}(0,y) =
\frac{kq}{(a^2+y^2)^{3/2}}
\left[
-a\hat{i} + 3y\hat{j}
\right]
$$

### 3. Field on the $x$-Axis: $\vec{E}(x,0)$

Set $y=0$:

$$
E_y = 0
$$

and

$$
E_x(x,0) =
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3}
$$

Therefore,

$$
\vec{E}(x,0) = E_x(x,0)\hat{i}
$$

### 4. Conditions for $E_x = 0$, $E_y = 0$, and $\vec{E}=0$

From the general formula:

$$
E_y =
kq y
\left[
\frac{1}{\left[(x+a)^2+y^2\right]^{3/2}}
+
\frac{2}{\left[(x-a)^2+y^2\right]^{3/2}}
\right]
$$

The bracket is always positive, so

$$
E_y = 0 \quad \Longrightarrow \quad y = 0
$$

Thus zero total field can occur only on the $x$-axis.

On the $x$-axis between the charges, with $-a < x < a$:

$$
E_x =
kq \frac{1}{(x+a)^2}
-
2kq \frac{1}{(a-x)^2}
$$

Set this equal to zero:

$$
\frac{1}{(x+a)^2} = \frac{2}{(a-x)^2}
$$

Take square roots:

$$
\frac{1}{x+a} = \frac{\sqrt{2}}{a-x}
$$

Thus,

$$
a - x = \sqrt{2}(x+a)
$$

Expand:

$$
a - x = \sqrt{2}x + \sqrt{2}a
$$

Group terms:

$$
a(1-\sqrt{2}) = x(1+\sqrt{2})
$$

Therefore,

$$
x = a \frac{1-\sqrt{2}}{1+\sqrt{2}}
$$

Rationalize:

$$
x = a(2\sqrt{2} - 3)
$$

This value lies between $-a$ and $a$, so it is the zero-field point.

### 5. Numerical Value for $\vec{E}(0,y)$

Given:

$$
a = 0.2 \text{ m}, \quad y = 0.3 \text{ m}, \quad q = 2 \times 10^{-6} \text{ C}
$$

Use

$$
\vec{E}(0,y) =
\frac{kq}{(a^2+y^2)^{3/2}}
\left[
-a\hat{i} + 3y\hat{j}
\right]
$$

First compute:

$$
a^2 + y^2 = 0.04 + 0.09 = 0.13
$$

$$
(0.13)^{3/2} \approx 0.0469
$$

Now:

$$
kq = (8.99 \times 10^9)(2 \times 10^{-6}) = 1.798 \times 10^4
$$

So the prefactor is

$$
\frac{kq}{(a^2+y^2)^{3/2}} \approx \frac{1.798 \times 10^4}{0.0469} \approx 3.83 \times 10^5
$$

Therefore,

$$
E_x \approx -(3.83 \times 10^5)(0.2) \approx -7.66 \times 10^4 \text{ N/C}
$$

$$
E_y \approx (3.83 \times 10^5)(0.9) \approx 3.45 \times 10^5 \text{ N/C}
$$

Hence,

$$
\vec{E}(0,0.3) \approx
(-7.66 \times 10^4)\hat{i} + (3.45 \times 10^5)\hat{j} \text{ N/C}
$$

### 6. Limit $y \gg a$

From

$$
\vec{E}(0,y) =
\frac{kq}{(a^2+y^2)^{3/2}}
\left[
-a\hat{i} + 3y\hat{j}
\right]
$$

if $y \gg a$, then

$$
(a^2+y^2)^{3/2} \approx y^3
$$

Thus

$$
\vec{E}(0,y) \approx kq
\left[
-\frac{a}{y^3}\hat{i} + \frac{3}{y^2}\hat{j}
\right]
$$

The vertical term dominates, so approximately

$$
\vec{E}(0,y) \approx \frac{3kq}{y^2}\hat{j}
$$

This is exactly the field of an effective total charge

$$
q_{\text{tot}} = 3q
$$

located near the origin.

## Final Result

General field:

$$
\vec{E}(x,y) =
kq \frac{(x+a)\hat{i} + y\hat{j}}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{(x-a)\hat{i} + y\hat{j}}{\left[(x-a)^2 + y^2\right]^{3/2}}
$$

Field on the $y$-axis:

$$
\vec{E}(0,y) =
\frac{kq}{(a^2+y^2)^{3/2}}
\left[
-a\hat{i} + 3y\hat{j}
\right]
$$

Zero field occurs on the $x$-axis at

$$
x = a(2\sqrt{2} - 3), \qquad y = 0
$$

For the numerical case:

$$
\vec{E}(0,0.3) \approx
(-7.66 \times 10^4)\hat{i} + (3.45 \times 10^5)\hat{j} \text{ N/C}
$$

For $y \gg a$:

$$
\vec{E}(0,y) \approx \frac{3kq}{y^2}\hat{j}
$$

## Interpretation

Close to the charges, the field reflects the asymmetry between $+q$ and $+2q$. Far away, the system behaves like a single effective charge of total value $3q$, so the field approaches that of one point charge located near the origin.