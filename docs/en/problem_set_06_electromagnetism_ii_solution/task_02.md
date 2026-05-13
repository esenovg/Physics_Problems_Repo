## Problem 2 — Velocity selection (crossed fields)

**Given:** $\vec{E}=(0,E,0)$, $\vec{B}=(0,0,B)$.

### 1. Condition for rectilinear motion

A charge moves in a straight line when the net force vanishes:

$$
\vec{F} = q\vec{E} + q\vec{v}\times\vec{B} = 0
$$

Assume the velocity is along $\hat{x}$: $\vec{v}=(v,0,0)$. Then:

$$
\vec{v}\times\vec{B} = (v,0,0)\times(0,0,B) = (0,-vB,0)
$$

The force balance becomes:

$$
q(0,E,0) + q(0,-vB,0) = 0 \quad\Longrightarrow\quad E = vB
$$

So the selected velocity is:

$$
\boxed{v_d = \frac{E}{B}}
$$

### 2. Numerical value

$$
v_d = \frac{400}{0.8} = 500\ \mathrm{m/s}
$$

### 3. Does kinetic energy change?

**No.** The net force is zero, so motion is uniform, and $E_k = \tfrac{1}{2}mv_d^2$ is constant.

### 4. Operating principle

The selector lets through **only those particles with $v=E/B$**. Faster particles experience a larger magnetic force than electric force and are deflected one way; slower particles are deflected the other way. Only particles with exactly $v=E/B$ pass through the slit undeflected. This is independent of the charge sign and mass — it selects purely by **speed**.