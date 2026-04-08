# Task 10 – Wave Sources Superposition

## Problem Statement

Create an animation of multiple wave sources described by

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_0}|^\alpha} \sin(k |\vec{r} - \vec{r_0}| - \omega t)
$$

where multiple sources contribute through superposition.

## Theory

Each point source emits a radial wave.

The total wave field is the sum:

$$
u_{\text{total}} = \sum_i u_i(\vec{r}, t)
$$

The factor

$$
\frac{1}{|\vec{r}-\vec{r_0}|^\alpha}
$$

controls amplitude decay:

- $\alpha = 0$ → no decay
- $\alpha = 1$ → physical spherical spreading
- $\alpha = 2$ → strong decay

## Step-by-Step Solution

### 1. Superposition Principle

The total displacement is

$$
u(\vec{r},t) = \sum_i \frac{A}{|\vec{r}-\vec{r_i}|^\alpha} \sin(k |\vec{r} - \vec{r_i}| - \omega t)
$$

### 2. Visualization Method

- each pixel corresponds to a spatial point
- distance to each source is calculated
- contributions are summed
- color represents amplitude

### 3. Interactive Elements

The simulation allows:

- placing sources with mouse click
- changing amplitude $A$
- adjusting decay parameter $\alpha$
- modifying wavelength $\lambda$
- observing interference patterns

## Final Result

The resulting pattern shows constructive and destructive interference between multiple sources.

## Interpretation

- overlapping waves create complex patterns
- phase differences determine interference
- amplitude decay affects visibility

## Interactive Simulation

See:
