# Task 02 – Harmonic Motion

## Problem Statement

A mass of $10$ kg attached to a spring oscillates according to

$$
x(t) = 0.2 \cos(10\pi t)
$$

where $x$ is measured in meters.

Determine:

1. the spring constant $k$
2. the total mechanical energy of the system

## Theory

The standard form of simple harmonic motion is

$$
x(t) = A \cos(\omega t + \phi)
$$

where:

- $A$ is the amplitude
- $\omega$ is the angular frequency
- $\phi$ is the phase constant

For a mass-spring system,

$$
\omega = \sqrt{\frac{k}{m}}
$$

which implies

$$
k = m\omega^2
$$

The total mechanical energy of a harmonic oscillator is constant and is given by

$$
E = \frac{1}{2}kA^2
$$

## Step-by-Step Solution

### 1. Identify the Parameters

Compare

$$
x(t) = 0.2 \cos(10\pi t)
$$

with the standard form

$$
x(t) = A\cos(\omega t + \phi)
$$

Thus,

$$
A = 0.2 \text{ m}
$$

and

$$
\omega = 10\pi \text{ rad/s}
$$

The mass is

$$
m = 10 \text{ kg}
$$

### 2. Calculate the Spring Constant

Use

$$
k = m\omega^2
$$

Substitute the known values:

$$
k = 10(10\pi)^2
$$

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2 \text{ N/m}
$$

Numerically,

$$
k \approx 1000 \cdot 9.8696 \approx 9869.6 \text{ N/m}
$$

### 3. Calculate the Total Mechanical Energy

Use

$$
E = \frac{1}{2}kA^2
$$

Substitute $k = 1000\pi^2$ and $A = 0.2$:

$$
E = \frac{1}{2}(1000\pi^2)(0.2)^2
$$

$$
E = \frac{1}{2}(1000\pi^2)(0.04)
$$

$$
E = 20\pi^2 \text{ J}
$$

Numerically,

$$
E \approx 20 \cdot 9.8696 \approx 197.4 \text{ J}
$$

## Final Result

Spring constant:

$$
k = 1000\pi^2 \text{ N/m} \approx 9869.6 \text{ N/m}
$$

Total mechanical energy:

$$
E = 20\pi^2 \text{ J} \approx 197.4 \text{ J}
$$

## Interpretation

The angular frequency determines how stiff the spring must be for a given mass. Since the oscillation frequency is high, the spring constant is large. The mechanical energy is fixed by the spring stiffness and the amplitude of oscillation.