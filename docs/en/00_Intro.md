# Task 01 – Vector Algebra

## Problem Statement

Two vectors in three-dimensional space are given:

$\vec{a} = [2, 1, -3]$

$\vec{b} = [4, -2, 1]$

Determine:

1. The magnitude of each vector
2. The dot product $\vec{a} \cdot \vec{b}$
3. The cross product $\vec{a} \times \vec{b}$
4. The angle between the vectors

---

## Theory

### Vector Magnitude

For a vector

$\vec{v} = [v_x, v_y, v_z]$

the magnitude is

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

---

### Dot Product

The dot product between two vectors is

$$
\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z
$$

It can also be expressed in terms of the angle $\theta$ between the vectors:

$$
\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta
$$

---

### Cross Product

The cross product produces a vector perpendicular to both vectors.

$$
\vec{a} \times \vec{b} =
\begin{pmatrix}
a_y b_z - a_z b_y \\
a_z b_x - a_x b_z \\
a_x b_y - a_y b_x
\end{pmatrix}
$$

---

## Step-by-Step Solution

### 1. Magnitude of $\vec{a}$

$$
|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| = \sqrt{4 + 1 + 9}
$$

$$
|\vec{a}| = \sqrt{14}
$$

---

### 2. Magnitude of $\vec{b}$

$$
|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| = \sqrt{16 + 4 + 1}
$$

$$
|\vec{b}| = \sqrt{21}
$$

---

### 3. Dot Product

$$
\vec{a} \cdot \vec{b}
=
(2)(4) + (1)(-2) + (-3)(1)
$$

$$
= 8 - 2 - 3
$$

$$
= 3
$$

---

### 4. Cross Product

$$
\vec{a} \times \vec{b}
=
\begin{pmatrix}
1(1) - (-3)(-2) \\
(-3)(4) - 2(1) \\
2(-2) - 1(4)
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 - 6 \\
-12 - 2 \\
-4 - 4
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-5 \\
-14 \\
-8
\end{pmatrix}
$$

---

### 5. Angle Between Vectors

Using

$$
\cos\theta =
\frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}
$$

Substituting values

$$
\cos\theta =
\frac{3}{\sqrt{14}\sqrt{21}}
$$

$$
\cos\theta =
\frac{3}{\sqrt{294}}
$$

Thus

$$
\theta =
\cos^{-1}\left(\frac{3}{\sqrt{294}}\right)
$$

---

## Final Result

Magnitudes

$$
|\vec{a}| = \sqrt{14}
$$

$$
|\vec{b}| = \sqrt{21}
$$

Dot product

$$
\vec{a} \cdot \vec{b} = 3
$$

Cross product

$$
\vec{a} \times \vec{b} =
\begin{pmatrix}
-5 \\
-14 \\
-8
\end{pmatrix}
$$

Angle

$$
\theta = \cos^{-1}\left(\frac{3}{\sqrt{294}}\right)
$$

---

## Interpretation

The positive dot product indicates that the angle between the vectors is less than $90^\circ$.  
The cross product vector represents a direction perpendicular to both original vectors according to the right-hand rule.


# Task 02 – Systems of Equations

## Problem Statement

Solve the system:

$2x + 3y = 12$

$x - y = 1$

---

## Theory

A system of linear equations can be solved by substitution or elimination.  
The substitution method expresses one variable in terms of another and substitutes it into the second equation.

---

## Step-by-Step Solution

From the second equation

$$
x - y = 1
$$

Solve for $x$

$$
x = y + 1
$$

Substitute into the first equation

$$
2(y + 1) + 3y = 12
$$

Expand

$$
2y + 2 + 3y = 12
$$

Combine terms

$$
5y + 2 = 12
$$

$$
5y = 10
$$

$$
y = 2
$$

Substitute back into

$$
x = y + 1
$$

$$
x = 2 + 1 = 3
$$

---

## Final Result

$$
x = 3
$$

$$
y = 2
$$

---

## Interpretation

The ordered pair $(3,2)$ satisfies both equations simultaneously and represents the intersection point of the two lines in the Cartesian plane.


# Task 03 – Proportionality

## Problem Statement

The gravitational force is

$F = G \frac{m_1 m_2}{r^2}$

Determine how the force changes if:

- $r$ is doubled
- both masses are halved.

---

## Theory

The gravitational force is directly proportional to the product of the masses and inversely proportional to the square of the distance.

$$
F \propto \frac{m_1 m_2}{r^2}
$$

---

## Step-by-Step Solution

Initial force

$$
F = G \frac{m_1 m_2}{r^2}
$$

New values

$$
m_1' = \frac{m_1}{2}
$$

$$
m_2' = \frac{m_2}{2}
$$

$$
r' = 2r
$$

Substitute into the formula

$$
F' =
G
\frac{(m_1/2)(m_2/2)}{(2r)^2}
$$

Simplify numerator

$$
= G \frac{m_1 m_2}{4}
$$

Simplify denominator

$$
(2r)^2 = 4r^2
$$

Thus

$$
F' =
G
\frac{m_1 m_2}{16 r^2}
$$

---

## Final Result

$$
F' = \frac{F}{16}
$$

---

## Interpretation

Halving both masses reduces the force by a factor of $4$, while doubling the distance reduces the force by another factor of $4$.  
The combined effect reduces the gravitational force by a factor of **16**.


# Task 04 – Rearranging Formulas

## Problem Statement

The period of a simple pendulum is

$T = 2\pi \sqrt{\frac{L}{g}}$

Rearrange the equation to solve for $g$.

---

## Theory

Algebraic rearrangement isolates the desired variable by applying inverse operations.

---

## Step-by-Step Solution

Start with

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Divide both sides by $2\pi$

$$
\frac{T}{2\pi} = \sqrt{\frac{L}{g}}
$$

Square both sides

$$
\left(\frac{T}{2\pi}\right)^2 = \frac{L}{g}
$$

Invert and multiply

$$
g = \frac{L}{\left(\frac{T}{2\pi}\right)^2}
$$

Simplify

$$
g = \frac{4\pi^2 L}{T^2}
$$

---

## Final Result

$$
g = \frac{4\pi^2 L}{T^2}
$$

---

## Interpretation

This formula allows experimental determination of gravitational acceleration by measuring the pendulum length and oscillation period.


# Task 05 – Trigonometry

## Problem Statement

A vector has magnitude $15$ and forms an angle of $60^\circ$ with the horizontal axis.  
Determine its horizontal and vertical components.

---

## Theory

Vector components are obtained using trigonometry.

$$
A_x = A \cos\theta
$$

$$
A_y = A \sin\theta
$$

---

## Step-by-Step Solution

Horizontal component

$$
A_x = 15 \cos 60^\circ
$$

$$
A_x = 15 \times 0.5
$$

$$
A_x = 7.5
$$

Vertical component

$$
A_y = 15 \sin 60^\circ
$$

$$
A_y = 15 \times \frac{\sqrt{3}}{2}
$$

$$
A_y = \frac{15\sqrt{3}}{2}
$$

---

## Final Result

$$
A_x = 7.5
$$

$$
A_y = \frac{15\sqrt{3}}{2}
$$

---

## Interpretation

The vector can be represented as

$$
\vec{A} = (7.5 , \frac{15\sqrt{3}}{2})
$$

which corresponds to its projection onto the horizontal and vertical axes.