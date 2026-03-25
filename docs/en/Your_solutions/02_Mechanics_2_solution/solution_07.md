# Task 07 – Dynamics with Friction

## Problem Statement

A $5$ kg block is placed on top of a $10$ kg block. A horizontal force of $45$ N is applied to the $10$ kg block. The $5$ kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is $0.2$.

Determine the acceleration of the $10$ kg block.

## Theory

The lower block experiences several horizontal forces:

1. the applied force to the right
2. kinetic friction from the upper block to the left
3. kinetic friction from the floor to the left

Newton's second law gives

$$
\sum F_x = ma
$$

Kinetic friction is

$$
f_k = \mu_k N
$$

## Step-by-Step Solution

### 1. Friction Between the Upper and Lower Blocks

The upper block has mass

$$
m_1 = 5 \text{ kg}
$$

Because it is tied to the wall while the lower block moves underneath it, the contact is sliding, so kinetic friction acts.

The normal force between the two blocks is

$$
N_1 = m_1 g
$$

Thus,

$$
N_1 = 5 \cdot 9.81 = 49.05 \text{ N}
$$

The friction magnitude is

$$
f_{k,1} = \mu_k N_1
$$

$$
f_{k,1} = 0.2 \cdot 49.05
$$

$$
f_{k,1} = 9.81 \text{ N}
$$

This force acts to the left on the lower block.

### 2. Friction Between the Lower Block and the Floor

The lower block has mass

$$
m_2 = 10 \text{ kg}
$$

The floor supports both blocks, so the normal force from the floor is

$$
N_2 = (m_1 + m_2)g
$$

$$
N_2 = (5 + 10) \cdot 9.81
$$

$$
N_2 = 147.15 \text{ N}
$$

Thus the floor friction is

$$
f_{k,2} = \mu_k N_2
$$

$$
f_{k,2} = 0.2 \cdot 147.15
$$

$$
f_{k,2} = 29.43 \text{ N}
$$

This also acts to the left.

### 3. Net Force on the Lower Block

The applied force is

$$
F = 45 \text{ N}
$$

The total resisting friction is

$$
f_{\text{total}} = f_{k,1} + f_{k,2}
$$

$$
f_{\text{total}} = 9.81 + 29.43
$$

$$
f_{\text{total}} = 39.24 \text{ N}
$$

Therefore, the net force on the $10$ kg block is

$$
F_{\text{net}} = 45 - 39.24
$$

$$
F_{\text{net}} = 5.76 \text{ N}
$$

### 4. Acceleration of the Lower Block

Apply Newton's second law to the lower block:

$$
F_{\text{net}} = m_2 a
$$

$$
5.76 = 10a
$$

$$
a = 0.576 \text{ m/s}^2
$$

## Final Result

The acceleration of the $10$ kg block is

$$
a = 0.576 \text{ m/s}^2
$$

## Interpretation

The applied force is almost completely opposed by friction from the floor and from the upper block. The system still moves, but only with a relatively small acceleration because most of the applied force is spent overcoming kinetic friction.