# Task 01 – Gravitational Dependence

## Problem Statement

A simple pendulum has a period of $4$ s on Earth.

1. Determine its period on the Moon, where gravitational acceleration is approximately $\frac{1}{6}$ of the Earth's value.
2. Determine the length required for a simple pendulum to have a period of exactly $1$ s on Earth.

## Theory

For small oscillations, the period of a simple pendulum is

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

For a fixed pendulum length $L$, the period is proportional to

$$
T \propto \frac{1}{\sqrt{g}}
$$

Thus, if gravity changes while the length remains the same, the ratio of periods is

$$
\frac{T_2}{T_1} = \sqrt{\frac{g_1}{g_2}}
$$

## Step-by-Step Solution

### Part 1 – Period on the Moon

On Earth,

$$
T_E = 4 \text{ s}
$$

On the Moon,

$$
g_M = \frac{g_E}{6}
$$

Using the proportionality relation,

$$
\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_M}}
$$

Substitute $g_M = \frac{g_E}{6}$:

$$
\frac{T_M}{4} = \sqrt{\frac{g_E}{g_E/6}}
$$

$$
\frac{T_M}{4} = \sqrt{6}
$$

Therefore,

$$
T_M = 4\sqrt{6}
$$

Numerically,

$$
T_M \approx 4 \cdot 2.449 \approx 9.80 \text{ s}
$$

### Part 2 – Length for a 1 s Pendulum on Earth

The desired period is

$$
T = 1 \text{ s}
$$

Using

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

solve for $L$.

Divide by $2\pi$:

$$
\frac{T}{2\pi} = \sqrt{\frac{L}{g}}
$$

Square both sides:

$$
\left(\frac{T}{2\pi}\right)^2 = \frac{L}{g}
$$

Multiply by $g$:

$$
L = g\left(\frac{T}{2\pi}\right)^2
$$

For Earth, take

$$
g = 9.81 \text{ m/s}^2
$$

Substitute $T = 1$ s:

$$
L = 9.81\left(\frac{1}{2\pi}\right)^2
$$

$$
L = \frac{9.81}{4\pi^2}
$$

Numerically,

$$
L \approx \frac{9.81}{39.478} \approx 0.248 \text{ m}
$$

## Final Result

Period on the Moon:

$$
T_M = 4\sqrt{6} \approx 9.80 \text{ s}
$$

Required pendulum length for $T=1$ s on Earth:

$$
L \approx 0.248 \text{ m}
$$

## Interpretation

A pendulum swings more slowly where gravity is weaker, because the restoring effect of gravity is reduced. On the Moon, the same pendulum takes much longer to complete one oscillation. The second result shows that a very short pendulum, about $24.8$ cm long, is needed to obtain a 1-second period on Earth.