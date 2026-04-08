# Task 08 – Traveling Wave Check

## Problem Statement

Determine which of the following functions can describe a traveling wave by checking whether they satisfy the wave equation

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}
$$

Functions:

a)

$$
y(x,t) = A\cos(kx^2 - \omega t)
$$

b)

$$
y(x,t) = A(x-vt)^2
$$

c)

$$
y(x,t) = A\log(x+vt)
$$

## Theory

A general traveling wave moving without change of shape can be written as

$$
y(x,t) = f(x-vt)
$$

or

$$
y(x,t) = f(x+vt)
$$

Such functions satisfy the one-dimensional wave equation, provided the required derivatives exist.

## Step-by-Step Solution

### Function a

Consider

$$
y(x,t) = A\cos(kx^2 - \omega t)
$$

The argument contains $x^2$, not the linear combination $x \pm vt$.

This already suggests that the shape is not translated rigidly along the $x$-axis.

A direct derivative check gives extra $x$-dependent terms that prevent the wave equation from being satisfied in the standard form.

Therefore, function a does not represent a traveling wave.

### Function b

Consider

$$
y(x,t) = A(x-vt)^2
$$

This has the form

$$
y(x,t) = f(x-vt)
$$

with

$$
f(u) = Au^2
$$

Now verify explicitly.

First derivatives:

$$
\frac{\partial y}{\partial x} = 2A(x-vt)
$$

$$
\frac{\partial^2 y}{\partial x^2} = 2A
$$

For time derivatives:

$$
\frac{\partial y}{\partial t} = 2A(x-vt)(-v)
$$

$$
\frac{\partial^2 y}{\partial t^2} = 2Av^2
$$

Then

$$
\frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = \frac{1}{v^2}(2Av^2) = 2A
$$

Thus,

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}
$$

So function b satisfies the wave equation.

### Function c

Consider

$$
y(x,t) = A\log(x+vt)
$$

This has the form

$$
y(x,t) = f(x+vt)
$$

with

$$
f(u) = A\log u
$$

Now verify.

First derivatives:

$$
\frac{\partial y}{\partial x} = \frac{A}{x+vt}
$$

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}
$$

Time derivatives:

$$
\frac{\partial y}{\partial t} = \frac{Av}{x+vt}
$$

$$
\frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}
$$

Therefore,

$$
\frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = -\frac{A}{(x+vt)^2}
$$

So

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}
$$

Hence function c also satisfies the wave equation.

## Final Result

Traveling waves:

- b) $y(x,t) = A(x-vt)^2$
- c) $y(x,t) = A\log(x+vt)$

Not a traveling wave:

- a) $y(x,t) = A\cos(kx^2 - \omega t)$

## Interpretation

A function represents a traveling wave when its shape depends only on $x-vt$ or $x+vt$. In such cases, the wave profile shifts in space without distortion. Function a fails because its dependence on $x^2$ changes the shape in a non-translational way.