# Task 08 – Work of a Variable Force

## Problem Statement

Given the one-dimensional force

$$
F(x) = -kx
$$

determine:

1. the equation of motion and its solution
2. the work done during the displacement from $0$ to $x_0$
3. the interpretation in terms of potential energy
4. the verification of the relation $F = -\frac{dU}{dx}$
5. the graphs of $F(x)$ and $U(x)$

## Theory

The force law

$$
F(x) = -kx
$$

is Hooke's law. It describes the restoring force of an ideal spring.

Newton's second law gives

$$
m\frac{d^2x}{dt^2} = -kx
$$

or equivalently,

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

This is the differential equation of simple harmonic motion.

The work done by a variable force from $x=a$ to $x=b$ is

$$
W = \int_a^b F(x)\,dx
$$

Potential energy is defined so that

$$
W_{a \to b} = U(a) - U(b)
$$

## Step-by-Step Solution

### 1. Equation of Motion

Starting from Newton's second law:

$$
m\frac{d^2x}{dt^2} = -kx
$$

Bring all terms to one side:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

Define

$$
\omega = \sqrt{\frac{k}{m}}
$$

Then the equation becomes

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

Its general solution is

$$
x(t) = A\cos(\omega t) + B\sin(\omega t)
$$

where $A$ and $B$ are constants determined by initial conditions.

### 2. Work Done from $0$ to $x_0$

Use the definition of work:

$$
W = \int_0^{x_0} F(x)\,dx
$$

Substitute $F(x) = -kx$:

$$
W = \int_0^{x_0} -kx\,dx
$$

Factor out the constant:

$$
W = -k\int_0^{x_0} x\,dx
$$

Integrate:

$$
W = -k\left[\frac{x^2}{2}\right]_0^{x_0}
$$

$$
W = -k\left(\frac{x_0^2}{2} - 0\right)
$$

$$
W = -\frac{1}{2}kx_0^2
$$

### 3. Potential Energy

Choose the reference value

$$
U(0) = 0
$$

Since

$$
W_{0 \to x_0} = U(0) - U(x_0)
$$

we have

$$
-\frac{1}{2}kx_0^2 = 0 - U(x_0)
$$

Thus,

$$
U(x_0) = \frac{1}{2}kx_0^2
$$

Therefore, the potential energy function is

$$
U(x) = \frac{1}{2}kx^2
$$

### 4. Verify $F = -\frac{dU}{dx}$

Differentiate $U(x)$:

$$
\frac{dU}{dx} = \frac{d}{dx}\left(\frac{1}{2}kx^2\right)
$$

$$
\frac{dU}{dx} = kx
$$

Thus,

$$
-\frac{dU}{dx} = -kx
$$

which matches the original force law:

$$
F(x) = -kx
$$

### 5. Graphs of $F(x)$ and $U(x)$

The force function

$$
F(x) = -kx
$$

is a straight line through the origin with negative slope.

The potential energy function

$$
U(x) = \frac{1}{2}kx^2
$$

is an upward-opening parabola with minimum at $x=0$.

A simple Python script for plotting both functions is shown below.

```python
import numpy as np
import matplotlib.pyplot as plt

k = 1.0
x = np.linspace(-4, 4, 400)

F = -k * x
U = 0.5 * k * x**2

plt.figure()
plt.plot(x, F)
plt.xlabel("x")
plt.ylabel("F(x)")
plt.title("Force Function F(x) = -kx")
plt.grid(True)
plt.show()

plt.figure()
plt.plot(x, U)
plt.xlabel("x")
plt.ylabel("U(x)")
plt.title("Potential Energy U(x) = (1/2)kx^2")
plt.grid(True)
plt.show()
```

## Final Result

Equation of motion:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

General solution:

$$
x(t) = A\cos\left(\sqrt{\frac{k}{m}}\,t\right) + B\sin\left(\sqrt{\frac{k}{m}}\,t\right)
$$

Work from $0$ to $x_0$:

$$
W = -\frac{1}{2}kx_0^2
$$

Potential energy:

$$
U(x) = \frac{1}{2}kx^2
$$

Verified relation:

$$
F = -\frac{dU}{dx}
$$

## Interpretation

This is the standard model of an ideal spring. The force always points toward equilibrium, which is why it is called a restoring force. The potential energy is smallest at $x=0$ and increases quadratically with displacement, showing that larger displacements store more energy in the spring.