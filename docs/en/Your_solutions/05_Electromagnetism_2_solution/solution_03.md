# Task 03 – Biot-Savart Law

## Problem Statement

A small straight wire segment of length

$$
\ell = 0.1 \text{ m}
$$

carries current

$$
I = 3 \text{ A}
$$

The point $P$ is at distance

$$
r = 0.2 \text{ m}
$$

from the segment. The segment is perpendicular to the line connecting it to point $P$.

Determine the magnetic field at point $P$ due to this current segment.

## Theory

For a small current element, the Biot-Savart law gives

$$
dB = \frac{\mu_0}{4\pi}\frac{I\,d\ell \sin\theta}{r^2}
$$

If the current segment is perpendicular to the line joining it to the observation point, then

$$
\theta = 90^\circ
$$

and

$$
\sin\theta = 1
$$

For a short segment, we approximate

$$
d\ell \approx \ell
$$

so

$$
B \approx \frac{\mu_0}{4\pi}\frac{I\ell}{r^2}
$$

## Step-by-Step Solution

Substitute the known values:

$$
\mu_0 = 4\pi \times 10^{-7} \text{ T m/A}
$$

Thus

$$
\frac{\mu_0}{4\pi} = 10^{-7} \text{ T m/A}
$$

Now calculate:

$$
B = 10^{-7}\frac{(3)(0.1)}{(0.2)^2}
$$

First compute the denominator:

$$
(0.2)^2 = 0.04
$$

Then the numerator:

$$
3 \cdot 0.1 = 0.3
$$

So

$$
B = 10^{-7}\frac{0.3}{0.04}
$$

$$
B = 10^{-7}(7.5)
$$

$$
B = 7.5 \times 10^{-7} \text{ T}
$$

## Final Result

The magnetic field at point $P$ is

$$
B = 7.5 \times 10^{-7} \text{ T}
$$

## Interpretation

The magnetic field due to a small current element is directly proportional to the current and segment length, and inversely proportional to the square of the distance. Because the segment is perpendicular to the line to the observation point, the field is maximal for that geometry.