# Task 06 – Function Analysis

## Problem Statement

Consider the function

$f(x) = 3x^2 - 12x + 7$

Determine whether the function has a local maximum or a local minimum, and find its location.

## Theory

For a differentiable function, local extrema occur at critical points where the first derivative is zero:

$$
f'(x) = 0
$$

To classify the critical point, the second derivative is used:

- if $f''(x) > 0$, the function has a local minimum
- if $f''(x) < 0$, the function has a local maximum

A quadratic function of the form

$$
f(x) = ax^2 + bx + c
$$

has a parabola shape. If $a > 0$, the parabola opens upward and its vertex is a minimum.

## Step-by-Step Solution

Differentiate the function:

$$
f(x) = 3x^2 - 12x + 7
$$

$$
f'(x) = 6x - 12
$$

Set the derivative equal to zero:

$$
6x - 12 = 0
$$

$$
6x = 12
$$

$$
x = 2
$$

This is the critical point.

Now compute the second derivative:

$$
f''(x) = 6
$$

Since

$$
f''(x) = 6 > 0
$$

the critical point at $x=2$ is a local minimum.

Next, evaluate the function at $x=2$:

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
f(2) = 3 \cdot 4 - 24 + 7
$$

$$
f(2) = 12 - 24 + 7
$$

$$
f(2) = -5
$$

Therefore, the minimum point is

$$
(2,-5)
$$

## Final Result

The function has a local minimum at

$$
x = 2
$$

with value

$$
f(2) = -5
$$

Thus, the minimum point is

$$
(2,-5)
$$

There is no local maximum.

## Interpretation

Because the coefficient of $x^2$ is positive, the parabola opens upward. This guarantees that the vertex is the lowest point of the graph. Therefore, the function decreases until $x=2$ and increases after $x=2$.