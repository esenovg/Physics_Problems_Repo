## Problem 1 — Lorentz force

**Given data:**

$$
\vec{B} = (0,0,1)\ \mathrm{T}, \quad \vec{v} = (2,3,0)\ \mathrm{m/s}, \quad q = 1\ \mathrm{mC} = 10^{-3}\ \mathrm{C}
$$

### 1. Lorentz force $\vec{F}$

The Lorentz force on a charge moving in a magnetic field is:

$$
\vec{F} = q\,\vec{v} \times \vec{B}
$$

Computing the cross product:

$$
\vec{v} \times \vec{B} =
\begin{vmatrix}
\hat{x} & \hat{y} & \hat{z} \\
2 & 3 & 0 \\
0 & 0 & 1
\end{vmatrix}
= (3\cdot 1 - 0\cdot 0)\hat{x} - (2\cdot 1 - 0\cdot 0)\hat{y} + (2\cdot 0 - 3\cdot 0)\hat{z}
$$

$$
\vec{v} \times \vec{B} = (3, -2, 0)\ \mathrm{m\cdot T / s}
$$

Therefore:

$$
\boxed{\vec{F} = q(\vec{v}\times\vec{B}) = 10^{-3}\cdot(3,-2,0) = (3\times 10^{-3},\ -2\times 10^{-3},\ 0)\ \mathrm{N}}
$$

### 2. Equation of motion

Newton's second law gives:

$$
m\frac{d\vec{v}}{dt} = q\,\vec{v}\times\vec{B}
$$

With $\vec{B}=(0,0,B)$, expanding the cross product:

$$
\frac{dv_x}{dt} = \frac{qB}{m}v_y, \quad \frac{dv_y}{dt} = -\frac{qB}{m}v_x, \quad \frac{dv_z}{dt} = 0
$$

Defining the **cyclotron frequency** $\omega = \dfrac{qB}{m}$, the solution is circular motion in the $xy$-plane:

$$
v_x(t) = v_0\cos(\omega t + \varphi), \quad v_y(t) = -v_0\sin(\omega t + \varphi)
$$

where $v_0 = \sqrt{v_x^2+v_y^2} = \sqrt{4+9} = \sqrt{13}\ \mathrm{m/s}$.

From the initial condition $\vec{v}(0)=(2,3,0)$:

$$
\cos\varphi = \frac{2}{\sqrt{13}}, \quad \sin\varphi = -\frac{3}{\sqrt{13}}
$$

Integrating, with $\vec{r}(0)=(0,0,0)$, the trajectory is a circle in the $xy$-plane.

### 3. Magnitude $|\vec{F}|$

$$
|\vec{F}| = \sqrt{(3\times 10^{-3})^2 + (-2\times 10^{-3})^2} = 10^{-3}\sqrt{13} \approx 3.6\times 10^{-3}\ \mathrm{N}
$$

### 4. Does the magnetic force do work?

**No.** The magnetic force is always perpendicular to the velocity:

$$
\vec{F}\cdot\vec{v} = q(\vec{v}\times\vec{B})\cdot\vec{v} = 0
$$

Therefore $P = \vec{F}\cdot\vec{v} = 0$, and the kinetic energy is conserved.

### 5. Radius of trajectory for $m=0.01\ \mathrm{kg}$

The centripetal condition gives:

$$
\frac{mv^2}{r} = qvB \quad\Longrightarrow\quad r = \frac{mv}{qB}
$$

$$
r = \frac{0.01 \cdot \sqrt{13}}{10^{-3}\cdot 1} = 10\sqrt{13} \approx 36.06\ \mathrm{m}
$$

### 6. How does $r$ change when $B$ doubles?

Since $r \propto 1/B$:

$$
B \to 2B \quad\Longrightarrow\quad r \to \frac{r}{2}
$$

The radius is **halved**.