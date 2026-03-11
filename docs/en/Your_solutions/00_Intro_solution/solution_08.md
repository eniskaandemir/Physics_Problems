# Task 08 – Definite Integrals

## Problem Statement

Calculate the area under the curve of the function

$f(x) = \sin(x)$

from

$x = 0$

to

$x = \pi$

## Theory

The area under a curve on an interval $[a,b]$ is given by the definite integral

$$
\int_a^b f(x)\,dx
$$

For the sine function,

$$
\int \sin(x)\,dx = -\cos(x) + C
$$

Thus,

$$
\int_0^{\pi} \sin(x)\,dx
$$

is found by evaluating the antiderivative at the upper and lower limits.

## Step-by-Step Solution

Set up the definite integral:

$$
A = \int_0^{\pi} \sin(x)\,dx
$$

Find the antiderivative:

$$
\int \sin(x)\,dx = -\cos(x)
$$

Apply the limits:

$$
A = \left[-\cos(x)\right]_0^{\pi}
$$

Substitute the upper and lower bounds:

$$
A = -\cos(\pi) - \left(-\cos(0)\right)
$$

Use the trigonometric values

$$
\cos(\pi) = -1
$$

and

$$
\cos(0) = 1
$$

Then

$$
A = -(-1) - (-1)
$$

$$
A = 1 + 1
$$

$$
A = 2
$$

## Final Result

The area under the curve is

$$
2
$$

## Interpretation

On the interval from $0$ to $\pi$, the function $\sin(x)$ is nonnegative, so the definite integral equals the geometric area under the curve. The result shows that the total enclosed area is exactly $2$ square units.