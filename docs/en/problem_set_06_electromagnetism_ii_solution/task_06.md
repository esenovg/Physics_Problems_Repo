## Problem 6 — Rod on metal rails in a $\vec{B}$ field

**Given:** $m=0.20\ \mathrm{kg}$, $L=0.30\ \mathrm{m}$, $B=0.80\ \mathrm{T}$, $R=0.50\ \Omega$, $\alpha=25^\circ$, $g=9.81\ \mathrm{m/s^2}$.

### 1. EMF and current

$$
\mathcal{E}(v) = BLv, \quad I(v) = \frac{\mathcal{E}}{R} = \frac{BLv}{R}
$$

### 2. Magnetic braking force

The force on a current-carrying rod in a magnetic field is $F=BIL$. Substituting $I=BLv/R$:

$$
\boxed{F_{\text{mag}} = BIL = \frac{B^2L^2}{R}\,v}
$$

By Lenz's law, this force **opposes the motion** (acts up the incline).

### 3. Equation of motion

Along the incline, taking "down the slope" as positive:

$$
m\frac{dv}{dt} = mg\sin\alpha - \frac{B^2L^2}{R}v
$$

This has the form of damped motion with damping coefficient $\gamma = \dfrac{B^2L^2}{R}$:

$$
m\dot v + \gamma v = mg\sin\alpha
$$

### 4. Terminal velocity

At terminal velocity, $\dot v=0$:

$$
mg\sin\alpha = \frac{B^2L^2}{R}v_\infty \quad\Longrightarrow\quad v_\infty = \frac{mgR\sin\alpha}{B^2L^2}
$$

Numerically:

$$
v_\infty = \frac{0.20\cdot 9.81\cdot 0.50\cdot \sin 25^\circ}{(0.80)^2\cdot(0.30)^2}
= \frac{0.20\cdot 9.81\cdot 0.50\cdot 0.4226}{0.0576}
\approx 7.20\ \mathrm{m/s}
$$

### 5. Power balance

At terminal velocity, gravitational power input equals Joule dissipation:

$$
P_{\text{grav}} = mg\sin\alpha\cdot v_\infty
$$

$$
P_{\text{Joule}} = I^2 R = \left(\frac{BLv_\infty}{R}\right)^2 R = \frac{B^2L^2 v_\infty^2}{R}
$$

Using $mg\sin\alpha = \dfrac{B^2L^2}{R}v_\infty$:

$$
mg\sin\alpha\cdot v_\infty = \frac{B^2L^2}{R}v_\infty^2 = I^2R \quad\checkmark
$$

All gravitational energy is converted into Joule heat in the resistance.