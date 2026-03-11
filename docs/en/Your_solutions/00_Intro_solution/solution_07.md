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