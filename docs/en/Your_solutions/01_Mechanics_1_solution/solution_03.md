# Task 03 – Path Intersection

## Problem Statement

Alice moves along the path

$$
A(t) = (2 + t,\; 8 - 3t)
$$

Bob moves along the path

$$
B(t) = (2t - 1,\; 2t + 2)
$$

Determine:

- whether their paths intersect
- if yes, when and where
- if not, the minimum distance and when it occurs

---

## Theory

Two objects collide if their positions are equal at the same time:

$$
A(t) = B(t)
$$

This gives a system of equations by equating coordinates.

---

## Step-by-Step Solution

### 1. Equate Coordinates

For intersection:

$$
2 + t = 2t - 1
$$

$$
8 - 3t = 2t + 2
$$

---

### 2. Solve First Equation

$$
2 + t = 2t - 1
$$

$$
2 + 1 = 2t - t
$$

$$
3 = t
$$

---

### 3. Check Second Equation

Substitute $t=3$:

$$
8 - 3(3) = 8 - 9 = -1
$$

$$
2(3) + 2 = 6 + 2 = 8
$$

Since

$$
-1 \neq 8
$$

the equations are inconsistent.

---

### 4. Conclusion

There is no time $t$ for which both coordinates match.

---

## Final Result

The paths do **not intersect**.

---

## Interpretation

Even though both objects move in the plane, their trajectories never coincide at the same time.  
Thus, no collision occurs.