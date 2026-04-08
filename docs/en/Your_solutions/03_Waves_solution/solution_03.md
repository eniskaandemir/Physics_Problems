# Task 03 – Superposition Principle

## Problem Statement

Two waves are given by

$$
y_1(x,t) = A\sin(kx - \omega t)
$$

and

$$
y_2(x,t) = A\sin(kx + \omega t)
$$

Determine:

1. the resulting standing wave
2. the positions of the nodes

## Theory

When two waves overlap, the total displacement is the sum:

$$
y(x,t) = y_1(x,t) + y_2(x,t)
$$

The trigonometric identity

$$
\sin(\alpha - \beta) + \sin(\alpha + \beta) = 2\sin\alpha \cos\beta
$$

is used to simplify the expression.

A node occurs where the amplitude is zero for all time.

## Step-by-Step Solution

Start with the sum:

$$
y(x,t) = A\sin(kx - \omega t) + A\sin(kx + \omega t)
$$

Factor out $A$:

$$
y(x,t) = A\left[\sin(kx - \omega t) + \sin(kx + \omega t)\right]
$$

Apply the identity with

$$
\alpha = kx
$$

and

$$
\beta = \omega t
$$

Then

$$
y(x,t) = 2A\sin(kx)\cos(\omega t)
$$

This is the standing-wave form.

### Nodes

Nodes occur where

$$
\sin(kx) = 0
$$

This happens when

$$
kx = n\pi
$$

where $n$ is any integer.

Thus,

$$
x_n = \frac{n\pi}{k}
$$

Since

$$
k = \frac{2\pi}{\lambda}
$$

we obtain

$$
x_n = \frac{n\lambda}{2}
$$

## Final Result

Standing wave:

$$
y(x,t) = 2A\sin(kx)\cos(\omega t)
$$

Nodes:

$$
x_n = \frac{n\pi}{k} = \frac{n\lambda}{2}
$$

## Interpretation

The two traveling waves move in opposite directions and interfere to form a standing wave. The nodes are fixed points where destructive interference occurs at all times.