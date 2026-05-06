# Task 14 – RLC Circuit

## Problem Statement

Write the differential equation for a series RLC circuit with:

- voltage source $V(t)$
- resistor $R$
- inductor $L$
- capacitor $C$

Assume the current is $I(t)$ and the capacitor charge is $Q(t)$.

Compare the equation with the damped harmonic oscillator.

## Theory

Kirchhoff’s voltage law states that the sum of voltage drops equals the source voltage:

$$ V(t) = V_R + V_L + V_C $$

The voltage drops are:

$$ V_R = RI $$

$$ V_L = L\frac{dI}{dt} $$

$$ V_C = \frac{Q}{C} $$

Current is related to charge by:

$$ I = \frac{dQ}{dt} $$

## Step-by-Step Solution

Substitute into Kirchhoff’s law:

$$ V(t) = RI + L\frac{dI}{dt} + \frac{Q}{C} $$

Use $I = \frac{dQ}{dt}$:

$$ V(t) = R\frac{dQ}{dt} + L\frac{d^2Q}{dt^2} + \frac{Q}{C} $$

Rearrange:

$$ L\frac{d^2Q}{dt^2} + R\frac{dQ}{dt} + \frac{1}{C}Q = V(t) $$

The damped harmonic oscillator equation is:

$$ m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F(t) $$

The analogies are:

$$ L \leftrightarrow m $$

$$ R \leftrightarrow b $$

$$ \frac{1}{C} \leftrightarrow k $$

$$ Q \leftrightarrow x $$

$$ V(t) \leftrightarrow F(t) $$

## Final Result

The series RLC equation is:

$$ L\frac{d^2Q}{dt^2} + R\frac{dQ}{dt} + \frac{1}{C}Q = V(t) $$

## Interpretation

The RLC circuit behaves mathematically like a damped harmonic oscillator. Inductance acts like inertia, resistance acts like damping, and capacitance provides the restoring effect.