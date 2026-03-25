# Task 09 – Vertical Throw with Drag

## Problem Statement

The motion is governed by

$$
m\frac{dv}{dt} = -mg - kv
$$

with initial conditions

$$
v(0) = v_0, \qquad x(0) = 10
$$

Determine:

1. the analytical solution for the velocity
2. the position as a function of time
3. the maximum height
4. a comparison with the case without drag
5. a numerical simulation in Python

## Theory

This is a first-order linear differential equation for velocity. It can be written as

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

Once $v(t)$ is found, position follows from integration:

$$
x(t) = x(0) + \int_0^t v(\tau)\,d\tau
$$

The maximum height occurs when the vertical velocity becomes zero:

$$
v(t_{\max}) = 0
$$

## Step-by-Step Solution

### 1. Solve the Velocity Equation

Start with

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

Let

$$
\lambda = \frac{k}{m}
$$

Then the equation becomes

$$
\frac{dv}{dt} + \lambda v = -g
$$

The homogeneous solution is

$$
v_h(t) = Ce^{-\lambda t}
$$

A constant particular solution satisfies

$$
0 + \lambda v_p = -g
$$

so

$$
v_p = -\frac{g}{\lambda} = -\frac{mg}{k}
$$

Therefore,

$$
v(t) = Ce^{-\lambda t} - \frac{mg}{k}
$$

Use the initial condition $v(0)=v_0$:

$$
v_0 = C - \frac{mg}{k}
$$

Thus,

$$
C = v_0 + \frac{mg}{k}
$$

So the velocity is

$$
v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-kt/m} - \frac{mg}{k}
$$

### 2. Determine the Position Function

Use

$$
x(t) = 10 + \int_0^t v(\tau)\,d\tau
$$

Substitute the expression for $v(\tau)$:

$$
x(t) = 10 + \int_0^t \left[\left(v_0 + \frac{mg}{k}\right)e^{-k\tau/m} - \frac{mg}{k}\right] d\tau
$$

Integrate term by term:

$$
\int_0^t e^{-k\tau/m}\,d\tau = \frac{m}{k}\left(1 - e^{-kt/m}\right)
$$

and

$$
\int_0^t 1\,d\tau = t
$$

Therefore,

$$
x(t) = 10 + \left(v_0 + \frac{mg}{k}\right)\frac{m}{k}\left(1 - e^{-kt/m}\right) - \frac{mg}{k}t
$$

### 3. Maximum Height

Maximum height occurs when $v(t)=0$:

$$
\left(v_0 + \frac{mg}{k}\right)e^{-kt/m} - \frac{mg}{k} = 0
$$

So

$$
\left(v_0 + \frac{mg}{k}\right)e^{-kt/m} = \frac{mg}{k}
$$

Then

$$
e^{-kt/m} = \frac{mg/k}{v_0 + mg/k}
$$

Take the natural logarithm:

$$
-\frac{k}{m}t_{\max} = \ln\left(\frac{mg/k}{v_0 + mg/k}\right)
$$

Thus,

$$
t_{\max} = \frac{m}{k}\ln\left(\frac{v_0 + mg/k}{mg/k}\right)
$$

This can be written more compactly as

$$
t_{\max} = \frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right)
$$

The maximum height is then

$$
x_{\max} = x(t_{\max})
$$

with $x(t)$ from the previous section.

### 4. Comparison with the Case Without Drag

Without drag, the velocity is

$$
v(t) = v_0 - gt
$$

and the maximum height above the launch point is

$$
h_{\max,\;0} = \frac{v_0^2}{2g}
$$

With drag, upward speed decreases faster because gravity and resistive force both act downward. Therefore:

- the time to reach the top is smaller
- the maximum height is smaller
- the full trajectory is lower than in vacuum

### 5. Numerical Simulation in Python

```python
import numpy as np
import matplotlib.pyplot as plt

m = 1.0
g = 9.81
k = 0.4
v0 = 20.0
x0 = 10.0

t = np.linspace(0, 5, 500)

v = (v0 + m*g/k) * np.exp(-k*t/m) - m*g/k
x = x0 + (v0 + m*g/k) * (m/k) * (1 - np.exp(-k*t/m)) - (m*g/k) * t

plt.figure()
plt.plot(t, v)
plt.xlabel("t")
plt.ylabel("v(t)")
plt.title("Velocity with Linear Drag")
plt.grid(True)
plt.show()

plt.figure()
plt.plot(t, x)
plt.xlabel("t")
plt.ylabel("x(t)")
plt.title("Vertical Position with Linear Drag")
plt.grid(True)
plt.show()
```

## Final Result

Velocity:

$$
v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-kt/m} - \frac{mg}{k}
$$

Position:

$$
x(t) = 10 + \left(v_0 + \frac{mg}{k}\right)\frac{m}{k}\left(1 - e^{-kt/m}\right) - \frac{mg}{k}t
$$

Time to maximum height:

$$
t_{\max} = \frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right)
$$

Maximum height:

$$
x_{\max} = x(t_{\max})
$$

## Interpretation

Linear drag reduces the upward velocity exponentially toward a terminal-like behavior. Compared with motion without drag, the particle rises for a shorter time and reaches a lower maximum height because some mechanical energy is dissipated by the resistive force.