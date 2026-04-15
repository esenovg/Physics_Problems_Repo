# Problem 5 — Momentum and one-dimensional head-on collision

We consider a **one-dimensional elastic collision** of two bodies with masses $m_1$ and $m_2$.  
Before the collision, their velocities are $u_1$ and $u_2$.  
After the collision, their velocities are $v_1$ and $v_2$.

---

## 1. Conservation laws

For an elastic collision in one dimension, both **momentum** and **kinetic energy** are conserved.

### Conservation of momentum

$$
m_1 u_1 + m_2 u_2 = m_1 v_1 + m_2 v_2
$$

### Conservation of kinetic energy

$$
\begin{aligned}
\frac{1}{2} m_1 u_1^2 + \frac{1}{2} m_2 u_2^2
&=
\frac{1}{2} m_1 v_1^2 + \frac{1}{2} m_2 v_2^2
\end{aligned}
$$

Multiplying the second equation by $$2$$ gives

$$
m_1 u_1^2 + m_2 u_2^2 = m_1 v_1^2 + m_2 v_2^2
$$

---

## 2. Derivation of the velocities after collision

We start from the momentum equation:

$$
m_1 (u_1 - v_1) = m_2 (v_2 - u_2)
$$

From the energy equation:

$$
m_1 (u_1^2 - v_1^2) = m_2 (v_2^2 - u_2^2)
$$

Factor both sides:

$$
m_1 (u_1 - v_1)(u_1 + v_1) = m_2 (v_2 - u_2)(v_2 + u_2)
$$

Using the momentum relation

$$
m_1 (u_1 - v_1) = m_2 (v_2 - u_2)
$$

we can divide both sides by this common factor and obtain

$$
u_1 + v_1 = v_2 + u_2
$$

Hence,

$$
u_1 - u_2 = -(v_1 - v_2)
$$

This means:

> In a one-dimensional elastic collision, the relative velocity of approach equals the negative of the relative velocity of separation.

Now solve the system

$$
m_1 u_1 + m_2 u_2 = m_1 v_1 + m_2 v_2
$$

$$
u_1 - u_2 = -(v_1 - v_2)
$$

The final formulas are:

### Velocity of body 1 after collision

$$
v_1 =
\frac{m_1 - m_2}{m_1 + m_2} u_1
+
\frac{2m_2}{m_1 + m_2} u_2
$$

### Velocity of body 2 after collision

$$
v_2 =
\frac{2m_1}{m_1 + m_2} u_1
+
\frac{m_2 - m_1}{m_1 + m_2} u_2
$$

These are the standard formulas for a one-dimensional elastic collision.

---

## 3. Special case: $$m_1 = m_2$$

Let

$$
m_1 = m_2 = m
$$

Then the formulas simplify to

$$
v_1 = u_2
$$

$$
v_2 = u_1
$$

### Interpretation

If the masses are equal, the bodies simply **exchange velocities**.

This is a very important physical result.  
For example, if the second body is initially at rest, so that

$$
u_2 = 0
$$

then after collision:

$$
v_1 = 0, \qquad v_2 = u_1
$$

So the first body stops, and the second body moves away with the original velocity of the first one.

This is exactly what is observed in collisions of equal billiard balls.

---

## 4. Limit case: $$m_2 \gg m_1$$

Now consider the case where the second mass is much larger than the first:

$$
m_2 \gg m_1
$$

We examine the formulas in this limit.

### Velocity of body 1

Starting from

$$
v_1 =
\frac{m_1 - m_2}{m_1 + m_2} u_1
+
\frac{2m_2}{m_1 + m_2} u_2
$$

when $$m_2 \gg m_1$$, we approximate:

$$
\frac{m_1 - m_2}{m_1 + m_2} \approx -1
$$

and

$$
\frac{2m_2}{m_1 + m_2} \approx 2
$$

Thus,

$$
v_1 \approx -u_1 + 2u_2
$$

### Velocity of body 2

For the second body:

$$
v_2 =
\frac{2m_1}{m_1 + m_2} u_1
+
\frac{m_2 - m_1}{m_1 + m_2} u_2
$$

Since $$m_1/m_2 \to 0$$, we get

$$
\frac{2m_1}{m_1 + m_2} \approx 0
$$

and

$$
\frac{m_2 - m_1}{m_1 + m_2} \approx 1
$$

Therefore,

$$
v_2 \approx u_2
$$

### Interpretation

The heavy body practically does not change its velocity, while the light body rebounds.

If additionally the heavy body is initially at rest, so that

$$
u_2 = 0
$$

then

$$
v_1 \approx -u_1
$$

$$
v_2 \approx 0
$$

So the lighter body bounces back with almost the same speed, while the heavier body remains almost unaffected.

This is physically similar to a small ball bouncing off a rigid wall.

---

## 5. Physical interpretation of the results

The formulas show how the outcome depends on the mass ratio.

### Case 1: Equal masses

$$
m_1 = m_2
$$

The velocities are exchanged:

$$
v_1 = u_2, \qquad v_2 = u_1
$$

This means momentum and energy are transferred very efficiently from one body to the other.

### Case 2: Very heavy target

$$
m_2 \gg m_1
$$

The heavy body behaves almost like an immovable obstacle.  
The lighter body reverses its motion approximately elastically.

### Case 3: Very light target

If instead

$$
m_1 \gg m_2
$$

then the first body is hardly affected, and the second body can leave with a much larger speed than it initially had.

This is another manifestation of conservation laws: the lighter object can gain a large velocity, even though the heavier one changes only slightly.

---

## 6. Final answer

For a one-dimensional elastic collision:

$$
m_1 u_1 + m_2 u_2 = m_1 v_1 + m_2 v_2
$$

$$
\begin{aligned}
\frac{1}{2} m_1 u_1^2 + \frac{1}{2} m_2 u_2^2
&=
\frac{1}{2} m_1 v_1^2 + \frac{1}{2} m_2 v_2^2
\end{aligned}
$$

and the velocities after collision are

$$
v_1 =
\frac{m_1 - m_2}{m_1 + m_2} u_1
+
\frac{2m_2}{m_1 + m_2} u_2
$$

$$
v_2 =
\frac{2m_1}{m_1 + m_2} u_1
+
\frac{m_2 - m_1}{m_1 + m_2} u_2
$$

For equal masses:

$$
v_1 = u_2, \qquad v_2 = u_1
$$

For $$m_2 \gg m_1$$:

$$
v_1 \approx -u_1 + 2u_2, \qquad v_2 \approx u_2
$$

and if additionally $$u_2 = 0$$:

$$
v_1 \approx -u_1, \qquad v_2 \approx 0
$$

---

## 7. Short conclusion

A one-dimensional elastic collision is governed by two conservation laws: momentum and kinetic energy.  
These laws uniquely determine the velocities after impact. The special cases clearly show the physical meaning:

- equal masses exchange velocities,
- a very light body rebounds from a very heavy one,
- the mass ratio determines how momentum and energy are redistributed.
