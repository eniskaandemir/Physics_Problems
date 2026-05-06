# Task 14 – RLC Circuit

## Problem Statement

Write the differential equation for a series RLC circuit containing:

- resistor $R$
- inductor $L$
- capacitor $C$
- voltage source $V(t)$

Compare the equation with the damped harmonic oscillator equation.

## Theory

Using Kirchhoff’s voltage law, the sum of voltage drops around the loop equals the applied voltage.

The voltage drops are:

### Resistor

$$
V_R = RI
$$

### Inductor

$$
V_L = L\frac{dI}{dt}
$$

### Capacitor

$$
V_C = \frac{Q}{C}
$$

where

$$
I = \frac{dQ}{dt}
$$

## Step-by-Step Solution

### 1. Kirchhoff’s Voltage Law

Apply KVL:

$$
V(t)
=
V_R + V_L + V_C
$$

Substitute expressions:

$$
V(t)
=
RI + L\frac{dI}{dt} + \frac{Q}{C}
$$

Using

$$
I = \frac{dQ}{dt}
$$

gives

$$
V(t)
=
R\frac{dQ}{dt}
+
L\frac{d^2Q}{dt^2}
+
\frac{Q}{C}
$$

Rearrange:

$$
L\frac{d^2Q}{dt^2}
+
R\frac{dQ}{dt}
+
\frac{1}{C}Q
=
V(t)
$$

### 2. Comparison with Damped Harmonic Oscillator

The damped harmonic oscillator equation is

$$
m\frac{d^2x}{dt^2}
+
b\frac{dx}{dt}
+
kx
=
F(t)
$$

Compare term by term:

$$
m \leftrightarrow L
$$

$$
b \leftrightarrow R
$$

$$
k \leftrightarrow \frac{1}{C}
$$

$$
x \leftrightarrow Q
$$

$$
F(t) \leftrightarrow V(t)
$$

## Final Result

The differential equation of a series RLC circuit is

$$
L\frac{d^2Q}{dt^2}
+
R\frac{dQ}{dt}
+
\frac{1}{C}Q
=
V(t)
$$

## Interpretation

The RLC circuit behaves mathematically like a damped harmonic oscillator.

- inductance acts like mass
- resistance acts like damping
- capacitance provides the restoring effect

This analogy is fundamental in both electrical engineering and physics.