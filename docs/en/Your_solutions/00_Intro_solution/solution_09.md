# Task 09 – Optimization Problem

## Problem Statement

A rectangle is placed under the curve

$y = 3 - x^2$

in the first quadrant.

Determine the dimensions of the rectangle with maximum area.

## Theory

A rectangle in the first quadrant under the curve can be described by:

- width $x$
- height $y = 3 - x^2$

Its area is therefore

$$
A(x) = x(3 - x^2)
$$

To maximize the area, differentiate $A(x)$ and solve

$$
A'(x) = 0
$$

Then use the second derivative or sign analysis to confirm that the critical point gives a maximum.

## Step-by-Step Solution

### Geometric Setup

Since the upper-right corner of the rectangle lies on the curve

$$
y = 3 - x^2
$$

the rectangle has:

$$
\text{width} = x
$$

$$
\text{height} = 3 - x^2
$$

Its area is

$$
A(x) = x(3 - x^2)
$$

Expand the expression:

$$
A(x) = 3x - x^3
$$

### Differentiate the Area Function

Compute the derivative:

$$
A'(x) = 3 - 3x^2
$$

Set the derivative equal to zero:

$$
3 - 3x^2 = 0
$$

$$
1 - x^2 = 0
$$

$$
x^2 = 1
$$

$$
x = 1
$$

Only the positive solution is valid because the rectangle is in the first quadrant.

### Determine the Height

Substitute $x=1$ into the curve equation:

$$
y = 3 - x^2
$$

$$
y = 3 - 1^2
$$

$$
y = 2
$$

### Verify Maximum

Differentiate again:

$$
A''(x) = -6x
$$

At $x=1$:

$$
A''(1) = -6
$$

Since

$$
A''(1) < 0
$$

the area is maximized at this point.

### Maximum Area

Compute the maximum area:

$$
A_{\max} = xy
$$

$$
A_{\max} = 1 \cdot 2
$$

$$
A_{\max} = 2
$$

## Final Result

The rectangle with maximum area has dimensions

$$
\text{width} = 1
$$

and

$$
\text{height} = 2
$$

Its maximum area is

$$
2
$$

## Interpretation

As the rectangle becomes wider, its height decreases because the top-right corner must remain on the parabola. The maximum-area rectangle occurs at the balance point where the gain in width no longer compensates for the loss in height.