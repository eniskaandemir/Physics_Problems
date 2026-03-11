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


# Task 06 – Function Analysis

## Problem Statement

Consider the function

$f(x) = 3x^2 - 12x + 7$

Determine whether the function has a local maximum or a local minimum, and find its location.

## Theory

For a differentiable function, local extrema occur at critical points where the first derivative is zero:

$$
f'(x) = 0
$$

To classify the critical point, the second derivative is used:

- if $f''(x) > 0$, the function has a local minimum
- if $f''(x) < 0$, the function has a local maximum

A quadratic function of the form

$$
f(x) = ax^2 + bx + c
$$

has a parabola shape. If $a > 0$, the parabola opens upward and its vertex is a minimum.

## Step-by-Step Solution

Differentiate the function:

$$
f(x) = 3x^2 - 12x + 7
$$

$$
f'(x) = 6x - 12
$$

Set the derivative equal to zero:

$$
6x - 12 = 0
$$

$$
6x = 12
$$

$$
x = 2
$$

This is the critical point.

Now compute the second derivative:

$$
f''(x) = 6
$$

Since

$$
f''(x) = 6 > 0
$$

the critical point at $x=2$ is a local minimum.

Next, evaluate the function at $x=2$:

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
f(2) = 3 \cdot 4 - 24 + 7
$$

$$
f(2) = 12 - 24 + 7
$$

$$
f(2) = -5
$$

Therefore, the minimum point is

$$
(2,-5)
$$

## Final Result

The function has a local minimum at

$$
x = 2
$$

with value

$$
f(2) = -5
$$

Thus, the minimum point is

$$
(2,-5)
$$

There is no local maximum.

## Interpretation

Because the coefficient of $x^2$ is positive, the parabola opens upward. This guarantees that the vertex is the lowest point of the graph. Therefore, the function decreases until $x=2$ and increases after $x=2$.


# Task 07 – Logic and Series

## Problem Statement

A bicycle is initially $10 \text{ m}$ from a wall and moves toward the wall at a constant speed of $1 \text{ m/s}$. A fly starts from the bicycle's front wheel and flies toward the wall at $2 \text{ m/s}$. Each time the fly reaches the wall, it immediately turns around and flies back toward the bicycle, repeating this process until the bicycle reaches the wall.

Determine the total distance traveled by the fly before it is crushed.

## Theory

This type of problem can be approached in two ways:

1. By summing an infinite sequence of back-and-forth distances
2. By using total time of motion

The second method is more direct. If the fly moves continuously until the bicycle reaches the wall, then

$$
\text{distance traveled by fly} = \text{fly speed} \times \text{total time}
$$

## Step-by-Step Solution

The bicycle starts $10 \text{ m}$ from the wall and moves at speed

$$
v_{\text{bike}} = 1 \text{ m/s}
$$

The time required for the bicycle to reach the wall is

$$
t = \frac{\text{distance}}{\text{speed}}
$$

Substitute the known values:

$$
t = \frac{10}{1}
$$

$$
t = 10 \text{ s}
$$

The fly travels during the entire $10 \text{ s}$ interval at constant speed

$$
v_{\text{fly}} = 2 \text{ m/s}
$$

Therefore, the total distance traveled by the fly is

$$
d_{\text{fly}} = v_{\text{fly}} t
$$

$$
d_{\text{fly}} = 2 \cdot 10
$$

$$
d_{\text{fly}} = 20 \text{ m}
$$

## Final Result

The fly travels a total distance of

$$
20 \text{ m}
$$

before being crushed.

## Interpretation

Although the fly changes direction infinitely many times, the total motion lasts only until the bicycle reaches the wall. Since that takes $10$ seconds, the problem reduces to uniform motion of the fly over that time interval. The infinite turning process does not change the total distance result.


# Task 08 – Definite Integrals

## Problem Statement

Calculate the area under the curve of the function

$f(x) = \sin(x)$

from

$x = 0$

to

$x = \pi$

## Theory

The area under a curve on an interval $[a,b]$ is given by the definite integral

$$
\int_a^b f(x)\,dx
$$

For the sine function,

$$
\int \sin(x)\,dx = -\cos(x) + C
$$

Thus,

$$
\int_0^{\pi} \sin(x)\,dx
$$

is found by evaluating the antiderivative at the upper and lower limits.

## Step-by-Step Solution

Set up the definite integral:

$$
A = \int_0^{\pi} \sin(x)\,dx
$$

Find the antiderivative:

$$
\int \sin(x)\,dx = -\cos(x)
$$

Apply the limits:

$$
A = \left[-\cos(x)\right]_0^{\pi}
$$

Substitute the upper and lower bounds:

$$
A = -\cos(\pi) - \left(-\cos(0)\right)
$$

Use the trigonometric values

$$
\cos(\pi) = -1
$$

and

$$
\cos(0) = 1
$$

Then

$$
A = -(-1) - (-1)
$$

$$
A = 1 + 1
$$

$$
A = 2
$$

## Final Result

The area under the curve is

$$
2
$$

## Interpretation

On the interval from $0$ to $\pi$, the function $\sin(x)$ is nonnegative, so the definite integral equals the geometric area under the curve. The result shows that the total enclosed area is exactly $2$ square units.


# Task 09 – Optimization Problem

## Problem Statement

A rectangle is placed under the curve

$y = 3 - x^2$

in the first quadrant.

Determine the dimensions of the rectangle with maximum area.

## Theory

A rectangle in the first quadrant under the curve can be described by:

- width $x$
- height $y = 3 - x^2$

Its area is therefore

$$
A(x) = x(3 - x^2)
$$

To maximize the area, differentiate $A(x)$ and solve

$$
A'(x) = 0
$$

Then use the second derivative or sign analysis to confirm that the critical point gives a maximum.

## Step-by-Step Solution

### Geometric Setup

Since the upper-right corner of the rectangle lies on the curve

$$
y = 3 - x^2
$$

the rectangle has:

$$
\text{width} = x
$$

$$
\text{height} = 3 - x^2
$$

Its area is

$$
A(x) = x(3 - x^2)
$$

Expand the expression:

$$
A(x) = 3x - x^3
$$

### Differentiate the Area Function

Compute the derivative:

$$
A'(x) = 3 - 3x^2
$$

Set the derivative equal to zero:

$$
3 - 3x^2 = 0
$$

$$
1 - x^2 = 0
$$

$$
x^2 = 1
$$

$$
x = 1
$$

Only the positive solution is valid because the rectangle is in the first quadrant.

### Determine the Height

Substitute $x=1$ into the curve equation:

$$
y = 3 - x^2
$$

$$
y = 3 - 1^2
$$

$$
y = 2
$$

### Verify Maximum

Differentiate again:

$$
A''(x) = -6x
$$

At $x=1$:

$$
A''(1) = -6
$$

Since

$$
A''(1) < 0
$$

the area is maximized at this point.

### Maximum Area

Compute the maximum area:

$$
A_{\max} = xy
$$

$$
A_{\max} = 1 \cdot 2
$$

$$
A_{\max} = 2
$$

## Final Result

The rectangle with maximum area has dimensions

$$
\text{width} = 1
$$

and

$$
\text{height} = 2
$$

Its maximum area is

$$
2
$$

## Interpretation

As the rectangle becomes wider, its height decreases because the top-right corner must remain on the parabola. The maximum-area rectangle occurs at the balance point where the gain in width no longer compensates for the loss in height.


# Task 10 – Infinite Series

## Problem Statement

An ant starts at the origin and moves according to the pattern:

- $1 \text{ m}$ east
- $\frac{1}{2} \text{ m}$ north
- $\frac{1}{3} \text{ m}$ west
- $\frac{1}{4} \text{ m}$ south
- $\frac{1}{5} \text{ m}$ east

and so on.

Determine the final position of the ant.

## Theory

The motion alternates between horizontal and vertical directions:

- odd-numbered steps in the horizontal direction
- even-numbered steps in the vertical direction

The horizontal displacement is an alternating series:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots
$$

The vertical displacement is also an alternating series:

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
$$

These are standard infinite series.

The Leibniz series gives

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \frac{\pi}{4}
$$

Also,

$$
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \ln 2
$$

From this, the even-term alternating series can be derived.

## Step-by-Step Solution

### Horizontal Displacement

The ant moves horizontally on odd-numbered steps:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots
$$

This is the Leibniz series for arctangent:

$$
x = \frac{\pi}{4}
$$

### Vertical Displacement

The vertical motion is

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
$$

Factor out $\frac{1}{2}$:

$$
y = \frac{1}{2}\left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots \right)
$$

The expression in parentheses is the alternating harmonic series:

$$
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \ln 2
$$

Therefore,

$$
y = \frac{1}{2}\ln 2
$$

### Final Coordinate

The ant starts at the origin, so its final position is

$$
\left(\frac{\pi}{4}, \frac{1}{2}\ln 2\right)
$$

## Final Result

The final position of the ant is

$$
\left(\frac{\pi}{4}, \frac{1}{2}\ln 2\right)
$$

## Interpretation

The horizontal and vertical displacements both converge because the step lengths form alternating series with decreasing magnitudes. Even though the ant makes infinitely many moves, the total displacement approaches a finite point in the plane.