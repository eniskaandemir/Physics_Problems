# Task 06 – Electromagnetic Wave Analysis

## Problem Statement

An electromagnetic wave has electric field component

$$
E_y(x,t) = 100 \sin(10^7 x - \omega t) \text{ V/m}
$$

Determine:

1. the direction of propagation
2. the wavelength $\lambda$
3. the angular frequency $\omega$
4. the equation for the magnetic field component

## Theory

A plane electromagnetic wave of the form

$$
E = E_0 \sin(kx - \omega t)
$$

propagates in the positive $x$-direction.

The wave number is

$$
k = \frac{2\pi}{\lambda}
$$

and for electromagnetic waves in vacuum,

$$
\omega = ck
$$

where

$$
c = 3.0 \times 10^8 \text{ m/s}
$$

Also, the electric and magnetic fields satisfy

$$
E_0 = cB_0
$$

so

$$
B_0 = \frac{E_0}{c}
$$

If the electric field oscillates in the $y$-direction and the wave propagates along $+x$, then the magnetic field must oscillate along the $z$-direction so that

$$
\vec{E} \times \vec{B}
$$

points in the direction of propagation.

## Step-by-Step Solution

### 1. Direction of Propagation

The phase is

$$
10^7 x - \omega t
$$

A wave of the form

$$
f(kx - \omega t)
$$

moves in the positive $x$-direction.

Therefore, the wave propagates along

$$
+\hat{i}
$$

### 2. Wavelength

From the given equation,

$$
k = 10^7 \text{ rad/m}
$$

Use

$$
\lambda = \frac{2\pi}{k}
$$

Thus,

$$
\lambda = \frac{2\pi}{10^7}
$$

$$
\lambda \approx 6.28 \times 10^{-7} \text{ m}
$$

### 3. Angular Frequency

Use

$$
\omega = ck
$$

Substitute the values:

$$
\omega = (3.0 \times 10^8)(10^7)
$$

$$
\omega = 3.0 \times 10^{15} \text{ rad/s}
$$

### 4. Magnetic Field Component

The electric field amplitude is

$$
E_0 = 100 \text{ V/m}
$$

Therefore,

$$
B_0 = \frac{E_0}{c} = \frac{100}{3.0 \times 10^8}
$$

$$
B_0 \approx 3.33 \times 10^{-7} \text{ T}
$$

Since $\vec{E}$ is in the $y$-direction and propagation is along $+x$, the magnetic field must be in the $z$-direction.

Thus,

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - \omega t) \text{ T}
$$

## Final Result

Direction of propagation:

$$
+\hat{i}
$$

Wavelength:

$$
\lambda \approx 6.28 \times 10^{-7} \text{ m}
$$

Angular frequency:

$$
\omega = 3.0 \times 10^{15} \text{ rad/s}
$$

Magnetic field component:

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - \omega t) \text{ T}
$$

## Interpretation

The wave travels in the positive $x$-direction, with the electric field oscillating along $y$ and the magnetic field oscillating along $z$. The electric and magnetic fields are perpendicular to each other and to the direction of propagation.