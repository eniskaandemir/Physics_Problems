# Task 01 – Projectile Motion

## Problem Statement

A projectile is fired from the ground with initial velocity

$v_0 = 100 \text{ m/s}$

at an angle

$\theta = 37^\circ$

Neglect air resistance.

Determine:

- the differential equations of motion
- the time of flight
- the maximum height
- the range

---

## Theory

Projectile motion is analyzed by decomposing motion into horizontal and vertical components.

Horizontal motion:

- no acceleration

Vertical motion:

- constant acceleration due to gravity

$$
\vec{a} = (0, -g)
$$

---

## Step-by-Step Solution

### 1. Initial Velocity Components

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

Substitute values:

$$
v_{0x} = 100 \cos 37^\circ \approx 80
$$

$$
v_{0y} = 100 \sin 37^\circ \approx 60
$$

---

### 2. Differential Equations

Horizontal motion:

$$
\frac{d^2 x}{dt^2} = 0
$$

Vertical motion:

$$
\frac{d^2 y}{dt^2} = -g
$$

---

### 3. Time of Flight

Time is determined from vertical motion.

At landing:

$$
y = 0
$$

Use equation:

$$
y(t) = v_{0y} t - \frac{1}{2} g t^2
$$

Set equal to zero:

$$
0 = t(v_{0y} - \frac{1}{2} g t)
$$

Non-zero solution:

$$
t = \frac{2 v_{0y}}{g}
$$

$$
t = \frac{2 \cdot 60}{9.8}
$$

$$
t \approx 12.24 \text{ s}
$$

---

### 4. Maximum Height

Occurs when vertical velocity is zero:

$$
v_y = v_{0y} - g t = 0
$$

$$
t = \frac{v_{0y}}{g}
$$

Height:

$$
H = \frac{v_{0y}^2}{2g}
$$

$$
H = \frac{60^2}{2 \cdot 9.8}
$$

$$
H \approx 183.7 \text{ m}
$$

---

### 5. Range

$$
R = v_{0x} \cdot t
$$

$$
R = 80 \cdot 12.24
$$

$$
R \approx 979.2 \text{ m}
$$

---

## Final Result

Time of flight:

$$
t \approx 12.24 \text{ s}
$$

Maximum height:

$$
H \approx 183.7 \text{ m}
$$

Range:

$$
R \approx 979.2 \text{ m}
$$

---

## Interpretation

Projectile motion separates into independent horizontal and vertical motions.  
The vertical motion determines flight time, while horizontal velocity determines the range.