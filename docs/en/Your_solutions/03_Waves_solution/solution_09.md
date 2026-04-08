# Task 09 – Damped Harmonic Oscillator

## Problem Statement

The motion of a damped harmonic oscillator is described by

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

The task is to:

- write the general solution
- classify motion types
- analyze the effect of damping
- visualize the system using numerical simulation

## Theory

This is a second-order linear differential equation.

Define:

$$
\gamma = \frac{b}{2m}, \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

The characteristic equation is

$$
r^2 + \frac{b}{m}r + \frac{k}{m} = 0
$$

The behavior depends on the discriminant:

$$
b^2 - 4mk
$$

## Step-by-Step Solution

### 1. General Solution

There are three cases:

#### Underdamped ($b^2 < 4mk$)

$$
x(t) = e^{-\gamma t}\left(A\cos(\omega t) + B\sin(\omega t)\right)
$$

where

$$
\omega = \sqrt{\omega_0^2 - \gamma^2}
$$

#### Critically damped ($b^2 = 4mk$)

$$
x(t) = (A + Bt)e^{-\gamma t}
$$

#### Overdamped ($b^2 > 4mk$)

$$
x(t) = A e^{r_1 t} + B e^{r_2 t}
$$

where $r_1, r_2$ are real negative roots.

### 2. Physical Interpretation

- Underdamped: oscillatory decay
- Critically damped: fastest return without oscillation
- Overdamped: slow return without oscillation

### 3. Numerical Simulation (RK4)

The differential equation is converted into a system:

$$
\frac{dx}{dt} = v
$$

$$
\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x
$$

This system is solved numerically using the Runge–Kutta method.

## Final Result

The behavior of the system depends on the damping coefficient $b$:

- small $b$ → oscillations
- critical $b$ → fastest stabilization
- large $b$ → slow decay

## Interpretation

Damping removes energy from the system. As $b$ increases, oscillations disappear and the system returns to equilibrium more slowly.

## Interactive Simulation

See:
