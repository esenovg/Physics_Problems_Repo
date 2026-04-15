# Problem Set 3 — Mechanics II: Dynamics and Energy  
## Worked solutions

---

# Problem 1 — Newton's second law (constant force)

Given:

$$
m = 2 \ \mathrm{kg},
\qquad
\vec F = (6,2)\ \mathrm{N},
\qquad
\vec v(0) = (1,-1)\ \mathrm{\frac{m}{s}},
\qquad
\vec r(0) = (0,0)\ \mathrm{m}
$$

## 1. Acceleration

From Newton's second law:

$$
\vec F = m \vec a
$$

therefore

$$
\vec a = \frac{\vec F}{m} = \left(\frac{6}{2}, \frac{2}{2}\right) = (3,1)\ \mathrm{\frac{m}{s^2}}
$$

So:

$$
\boxed{\vec a(t) = (3,1)\ \mathrm{\frac{m}{s^2}}}
$$

It is constant.

## 2. Velocity

Integrating acceleration:

$$
\vec v(t) = \vec v(0) + \vec a\, t
$$

hence

$$
\boxed{\vec v(t) = (1+3t,\,-1+t)\ \mathrm{\frac{m}{s}}}
$$

## 3. Position

Integrating velocity:

$$
\vec r(t) = \vec r(0) + \vec v(0)t + \frac{1}{2}\vec a\, t^2
$$

thus

$$
\boxed{
\vec r(t) =
\left(
t + \frac{3}{2} t^2,\,
- t + \frac{1}{2} t^2
\right)\ \mathrm{m}
}
$$

So the coordinate form is

$$
\boxed{x(t)= t+\frac{3}{2}t^2}
$$

$$
\boxed{y(t)= -t+\frac{1}{2}t^2}
$$

## 4. Trajectory

The trajectory is given parametrically by

$$
x(t)= t+\frac{3}{2}t^2,
\qquad
y(t)= -t+\frac{1}{2}t^2
$$

This is a parabola in the plane.

A quick sketch can be made by evaluating a few points:

$$
t=0 \Rightarrow (x,y)=(0,0)
$$

$$
t=1 \Rightarrow (x,y)=\left(\frac{5}{2},-\frac{1}{2}\right)
$$

$$
t=2 \Rightarrow (x,y)=(8,0)
$$

$$
t=3 \Rightarrow (x,y)=\left(\frac{33}{2},\frac{3}{2}\right)
$$

So the body first moves downward, then turns upward in the vertical direction.

## 5. Work done by the force up to time $t=3\ \mathrm{s}$

The displacement at time $t=3$ is

$$
\Delta \vec r = \vec r(3) - \vec r(0)
$$

Since

$$
\vec r(3)=
\left(
3+\frac{3}{2}\cdot 9,\,
-3+\frac{1}{2}\cdot 9
\right)
=
\left(
\frac{33}{2},\,
\frac{3}{2}
\right)
$$

we get

$$
\Delta \vec r = \left(\frac{33}{2},\frac{3}{2}\right)
$$

Work done by a constant force:

$$
W = \vec F \cdot \Delta \vec r
$$

Therefore

$$
W = (6,2)\cdot \left(\frac{33}{2},\frac{3}{2}\right)
= 6\cdot \frac{33}{2} + 2\cdot \frac{3}{2}
= 99 + 3 = 102\ \mathrm{J}
$$

Hence

$$
\boxed{W(0\to 3\ \mathrm{s}) = 102\ \mathrm{J}}
$$

## 6. Check with the work-energy theorem

Initial kinetic energy:

$$
T_0 = \frac{1}{2}m |\vec v(0)|^2
= \frac{1}{2}\cdot 2 \cdot \left(1^2+(-1)^2\right)
= 2\ \mathrm{J}
$$

Velocity at $t=3$:

$$
\vec v(3) = (1+9,\,-1+3) = (10,2)
$$

Final kinetic energy:

$$
T_3 = \frac{1}{2}m |\vec v(3)|^2
= \frac{1}{2}\cdot 2 \cdot (10^2+2^2)
= 104\ \mathrm{J}
$$

So

$$
\Delta T = T_3 - T_0 = 104 - 2 = 102\ \mathrm{J}
$$

Thus

$$
\boxed{W = \Delta T}
$$

which confirms the work-energy theorem.

---

# Problem 2 — Inclined plane with friction

A body of mass $m$ slides down a plane of angle $\alpha$ with kinetic friction coefficient $\mu$.

## 1. Forces acting on the body

There are three forces:

1. Gravity:
$$
\vec F_g = m\vec g
$$

2. Normal reaction of the plane:
$$
\vec N
$$

3. Kinetic friction:
$$
\vec F_f
$$

The magnitude of the friction force is

$$
F_f = \mu N
$$

Choose axes:

- along the plane: $\hat s$,
- perpendicular to the plane: $\hat n$.

Components of gravity:

$$
mg\sin\alpha
\quad \text{along the plane}
$$

$$
mg\cos\alpha
\quad \text{perpendicular to the plane}
$$

Therefore

$$
N = mg\cos\alpha
$$

and

$$
F_f = \mu mg\cos\alpha
$$

## 2. Acceleration

Along the plane, Newton's second law gives

$$
ma = mg\sin\alpha - \mu mg\cos\alpha
$$

Hence

$$
\boxed{a = g(\sin\alpha - \mu\cos\alpha)}
$$

Vector form along the downward direction of the plane:

$$
\boxed{\vec a = g(\sin\alpha - \mu\cos\alpha)\,\hat s}
$$

For the body to actually slide downward, we need

$$
\sin\alpha - \mu\cos\alpha > 0
$$

that is

$$
\boxed{\tan\alpha > \mu}
$$

## 3. Time of descent from height $h$

If the vertical height is $h$, then the length of the path along the plane is

$$
L = \frac{h}{\sin\alpha}
$$

Assuming the body starts from rest:

$$
L = \frac{1}{2}at^2
$$

Therefore

$$
t = \sqrt{\frac{2L}{a}}
$$

Substituting for $L$ and $a$:

$$
\boxed{
t =
\sqrt{
\frac{2h}{
g\sin\alpha\,(\sin\alpha-\mu\cos\alpha)
}
}
}
$$

## 4. Final velocity

Using

$$
v^2 = 2aL
$$

we obtain

$$
v^2 = 2g(\sin\alpha-\mu\cos\alpha)\cdot \frac{h}{\sin\alpha}
$$

So

$$
\boxed{
v =
\sqrt{
2gh\left(1-\mu\cot\alpha\right)
}
}
$$

## 5. Check with energy balance

Initial potential energy:

$$
U_i = mgh
$$

Final kinetic energy:

$$
T_f = \frac{1}{2}mv^2
$$

Work done by friction:

$$
W_f = -F_f L = -\mu mg\cos\alpha \cdot \frac{h}{\sin\alpha}
= -\mu mgh\cot\alpha
$$

Energy balance:

$$
mgh + W_f = \frac{1}{2}mv^2
$$

Thus

$$
mgh - \mu mgh\cot\alpha = \frac{1}{2}mv^2
$$

which gives

$$
v^2 = 2gh(1-\mu\cot\alpha)
$$

This agrees exactly with the result from dynamics.

---

# Problem 3 — Work of a variable force

Given the one-dimensional force

$$
F(x) = -kx
$$

## 1. Equation of motion and its solution

Newton's second law gives

$$
m\ddot x = -kx
$$

or

$$
\boxed{m\ddot x + kx = 0}
$$

This is the harmonic oscillator equation.

Define

$$
\omega = \sqrt{\frac{k}{m}}
$$

Then the general solution is

$$
\boxed{
x(t) = A\cos(\omega t) + B\sin(\omega t)
}
$$

or equivalently

$$
\boxed{
x(t) = C\cos(\omega t + \phi)
}
$$

## 2. Work done during displacement from $0$ to $x_0$

Work is

$$
W = \int_0^{x_0} F(x)\,dx
$$

Therefore

$$
W = \int_0^{x_0} (-kx)\,dx
= -k\int_0^{x_0} x\,dx
= -k\left[\frac{x^2}{2}\right]_0^{x_0}
$$

So

$$
\boxed{
W(0\to x_0) = -\frac{1}{2}k x_0^2
}
$$

## 3. Interpretation as potential energy

For a conservative force,

$$
W = -\Delta U
$$

Choosing

$$
U(0)=0
$$

we get

$$
\boxed{
U(x)=\frac{1}{2}kx^2
}
$$

This is the elastic potential energy of a spring.

## 4. Verification of the relation $F = -\frac{dU}{dx}$

Differentiate the potential:

$$
\frac{dU}{dx} = \frac{d}{dx}\left(\frac{1}{2}kx^2\right)=kx
$$

Hence

$$
-\frac{dU}{dx} = -kx = F(x)
$$

Therefore

$$
\boxed{F(x)=-\frac{dU}{dx}}
$$

## 5. Graphs of $F(x)$ and $U(x)$

Force:

$$
F(x) = -kx
$$

This is a straight line through the origin with negative slope.

Potential energy:

$$
U(x)=\frac{1}{2}kx^2
$$

This is an upward-opening parabola with minimum at

$$
x=0
$$

---

# Problem 4 — Conservation of energy

A body falls freely from rest from initial height $H$ with no air resistance.

To avoid confusion, let:

- $H$ = initial height,
- $y$ = current height above the ground.

## 1. Total energy

Potential energy:

$$
U(y)=mgy
$$

Kinetic energy:

$$
T(y)=\frac{1}{2}mv^2
$$

Since the body starts from rest at height $H$:

$$
E = mgH
$$

At any height $y$:

$$
\boxed{
E = \frac{1}{2}mv^2 + mgy = mgH
}
$$

## 2. Velocity as a function of height

From energy conservation:

$$
\frac{1}{2}mv^2 + mgy = mgH
$$

Hence

$$
\frac{1}{2}mv^2 = mg(H-y)
$$

so

$$
v^2 = 2g(H-y)
$$

and therefore

$$
\boxed{
v(y)=\sqrt{2g(H-y)}
}
$$

## 3. Comparison with Newton's second law

From Newton's second law:

$$
m\ddot y = -mg
$$

so the acceleration is constant:

$$
\ddot y = -g
$$

Using the kinematic formula

$$
v^2 = v_0^2 + 2a(y-y_0)
$$

with

$$
v_0=0,
\qquad
a=-g,
\qquad
y_0=H
$$

we get

$$
v^2 = 2g(H-y)
$$

which is the same as the energy result.

## 4. At what height is kinetic energy equal to 75% of the total energy?

Total energy is constant:

$$
E = mgH
$$

If kinetic energy is $75\%$ of the total energy, then

$$
T = 0.75\,mgH
$$

Since

$$
U = E-T = 0.25\,mgH
$$

and

$$
U = mgy
$$

we obtain

$$
mgy = 0.25\,mgH
$$

thus

$$
\boxed{y=\frac{H}{4}}
$$

So the body has $75\%$ of its total energy as kinetic energy when it is at one quarter of the initial height above the ground.

---

# Problem 5 — Momentum and one-dimensional head-on collision

Let the initial velocities be:

$$
u_1,\qquad u_2
$$

and the final velocities after an elastic collision be:

$$
v_1,\qquad v_2
$$

## 1. Conservation laws

### Conservation of momentum

$$
\boxed{
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
}
$$

### Conservation of kinetic energy

$$
\boxed{
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
}
$$

## 2. Velocities after the collision

The standard result for a one-dimensional elastic collision is

$$
\boxed{
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
}
$$

$$
\boxed{
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
}
$$

## 3. Case $m_1=m_2$

If the masses are equal, then

$$
v_1 = u_2,
\qquad
v_2 = u_1
$$

So:

$$
\boxed{\text{for } m_1=m_2,\ \text{the bodies exchange velocities}}
$$

This is the familiar result from colliding identical balls.

## 4. Limit $m_2 \gg m_1$

Take the limit of a very heavy second body. Then

$$
v_1 \approx -u_1 + 2u_2
$$

$$
v_2 \approx u_2
$$

So the heavy body is practically unaffected, while the light body reflects from it.

In the especially important case

$$
u_2=0
$$

we get

$$
v_1 \approx -u_1,
\qquad
v_2 \approx 0
$$

Thus the light body rebounds with nearly the same speed in the opposite direction.

## 5. Physical interpretation

- Equal masses: velocities are exchanged.
- Very heavy target: the heavy body behaves almost like an immovable wall.
- Elasticity means that no kinetic energy is lost to heat or permanent deformation.

---

# Problem 6 — Motion with linear drag

The drag force is

$$
F = -kv
$$

with initial conditions

$$
v(0)=v_0,
\qquad
x(0)=0
$$

## 1. Equation of motion and solution

Newton's second law gives

$$
m\frac{dv}{dt} = -kv
$$

This can be written as

$$
\frac{dv}{v} = -\frac{k}{m}dt
$$

Integrating:

$$
\ln|v| = -\frac{k}{m}t + C
$$

Using the initial condition $v(0)=v_0$:

$$
\boxed{
v(t)=v_0 e^{-\frac{k}{m}t}
}
$$

Now integrate velocity to obtain position:

$$
x(t) = \int_0^t v_0 e^{-\frac{k}{m}\tau}\,d\tau
$$

Hence

$$
\boxed{
x(t)=\frac{mv_0}{k}\left(1-e^{-\frac{k}{m}t}\right)
}
$$

## 2. Limit as $t\to\infty$

For the velocity:

$$
\lim_{t\to\infty} v(t)
=
\lim_{t\to\infty} v_0 e^{-\frac{k}{m}t}
=0
$$

Therefore

$$
\boxed{
\lim_{t\to\infty} v(t)=0
}
$$

For the position:

$$
\lim_{t\to\infty} x(t)=\frac{mv_0}{k}
$$

So the body approaches a finite stopping distance.

## 3. Comparison with motion without drag

Without drag:

$$
m\frac{dv}{dt}=0
$$

thus

$$
v(t)=v_0
$$

and

$$
x(t)=v_0 t
$$

Comparison:

- without drag: constant velocity, distance grows linearly without bound,
- with drag: velocity decays exponentially to zero, position approaches a finite limit.

---

# Problem 7 — Vertical throw with drag

Given

$$
m\frac{dv}{dt} = -mg - kv
$$

with

$$
v(0)=v_0,
\qquad
x(0)=0
$$

Take the positive direction upward.

## 1. Solution of the equation

Rewrite:

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

Define

$$
\beta = \frac{k}{m}
$$

Then

$$
\frac{dv}{dt} + \beta v = -g
$$

The solution is

$$
\boxed{
v(t)=\left(v_0+\frac{g}{\beta}\right)e^{-\beta t}-\frac{g}{\beta}
}
$$

Returning to the original parameters:

$$
\boxed{
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-\frac{k}{m}t}-\frac{mg}{k}
}
$$

Now integrate to obtain the height:

$$
x(t)=\int_0^t v(\tau)\,d\tau
$$

Therefore

$$
\boxed{
x(t)=
\frac{1}{\beta}\left(v_0+\frac{g}{\beta}\right)\left(1-e^{-\beta t}\right)
-\frac{g}{\beta}t
}
$$

or equivalently

$$
\boxed{
x(t)=
\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-\frac{k}{m}t}\right)
-\frac{mg}{k}t
}
$$

## 2. Maximum height

At maximum height,

$$
v(t_\text{max})=0
$$

Thus

$$
\left(v_0+\frac{g}{\beta}\right)e^{-\beta t_\text{max}}-\frac{g}{\beta}=0
$$

So

$$
e^{-\beta t_\text{max}}
=
\frac{\frac{g}{\beta}}{v_0+\frac{g}{\beta}}
=
\frac{1}{1+\frac{\beta v_0}{g}}
$$

Hence

$$
\boxed{
t_\text{max}
=
\frac{1}{\beta}\ln\left(1+\frac{\beta v_0}{g}\right)
}
$$

or

$$
\boxed{
t_\text{max}
=
\frac{m}{k}\ln\left(1+\frac{kv_0}{mg}\right)
}
$$

Insert this into $x(t)$:

$$
\boxed{
x_\text{max}
=
\frac{v_0}{\beta}
-
\frac{g}{\beta^2}
\ln\left(1+\frac{\beta v_0}{g}\right)
}
$$

that is

$$
\boxed{
x_\text{max}
=
\frac{mv_0}{k}
-
\frac{m^2g}{k^2}
\ln\left(1+\frac{kv_0}{mg}\right)
}
$$

## 3. Comparison with the case without drag

Without drag:

$$
v(t)=v_0-gt
$$

$$
x(t)=v_0 t - \frac{1}{2}gt^2
$$

and

$$
x_\text{max}=\frac{v_0^2}{2g}
$$

With drag:

- the upward velocity decreases faster,
- the maximum height is smaller,
- the ascent time is shorter.

As a consistency check, when

$$
k\to 0
$$

the formulas reduce to the drag-free results.

## 4. Numerical simulation

A numerical simulation solves the system

$$
\frac{dx}{dt}=v
$$

$$
\frac{dv}{dt}=-g-\frac{k}{m}v
$$

A simple Python program:

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp

m = 1.0
k = 0.4
g = 9.81
v0 = 20.0

def rhs(t, y):
    x, v = y
    return [v, -g - (k/m)*v]

t_span = (0, 5)
t_eval = np.linspace(*t_span, 400)

sol = solve_ivp(rhs, t_span, [0.0, v0], t_eval=t_eval)

t = sol.t
x_num = sol.y[0]
v_num = sol.y[1]

beta = k/m
v_ana = (v0 + g/beta) * np.exp(-beta*t) - g/beta
x_ana = ((v0 + g/beta) / beta) * (1 - np.exp(-beta*t)) - (g/beta) * t

plt.figure(figsize=(8, 4))
plt.plot(t, x_num, label="numerical x(t)")
plt.plot(t, x_ana, "--", label="analytical x(t)")
plt.xlabel("t")
plt.ylabel("x")
plt.legend()
plt.grid()
plt.show()

plt.figure(figsize=(8, 4))
plt.plot(t, v_num, label="numerical v(t)")
plt.plot(t, v_ana, "--", label="analytical v(t)")
plt.xlabel("t")
plt.ylabel("v")
plt.legend()
plt.grid()
plt.show()
```

## 5. Comparison of analytical and numerical solutions

For this linear problem, the numerical and analytical solutions should overlap almost perfectly if the numerical step is sufficiently small.

That agreement confirms that:

- the analytical derivation is correct,
- the numerical method is implemented correctly.

---

# Problem 8 — Harmonic oscillator (formal dynamics)

Given

$$
m\ddot x + kx = 0
$$

## 1. Solution of the equation

Rewrite as

$$
\ddot x + \frac{k}{m}x = 0
$$

Define the natural angular frequency:

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Then

$$
\ddot x + \omega_0^2 x = 0
$$

The general solution is

$$
\boxed{
x(t)=A\cos(\omega_0 t)+B\sin(\omega_0 t)
}
$$

or

$$
\boxed{
x(t)=C\cos(\omega_0 t+\phi)
}
$$

## 2. Natural frequency

Angular frequency:

$$
\boxed{
\omega_0=\sqrt{\frac{k}{m}}
}
$$

Ordinary frequency:

$$
\boxed{
f=\frac{\omega_0}{2\pi}
=
\frac{1}{2\pi}\sqrt{\frac{k}{m}}
}
$$

## 3. Energy as a function of time

Kinetic energy:

$$
T=\frac{1}{2}m\dot x^2
$$

Potential energy:

$$
U=\frac{1}{2}kx^2
$$

Hence total energy:

$$
\boxed{
E(t)=\frac{1}{2}m\dot x^2+\frac{1}{2}kx^2
}
$$

Using

$$
x(t)=C\cos(\omega_0 t+\phi)
$$

we have

$$
\dot x(t)=-C\omega_0\sin(\omega_0 t+\phi)
$$

Therefore

$$
E(t)=
\frac{1}{2}m C^2\omega_0^2\sin^2(\omega_0 t+\phi)
+
\frac{1}{2}k C^2\cos^2(\omega_0 t+\phi)
$$

Since

$$
m\omega_0^2 = k
$$

we get

$$
E(t)=
\frac{1}{2}kC^2\sin^2(\omega_0 t+\phi)
+
\frac{1}{2}kC^2\cos^2(\omega_0 t+\phi)
$$

thus

$$
\boxed{
E(t)=\frac{1}{2}kC^2=\mathrm{const}
}
$$

## 4. Proof that energy is conserved

Differentiate the total energy:

$$
\frac{dE}{dt}
=
m\dot x\ddot x + kx\dot x
=
\dot x(m\ddot x + kx)
$$

But from the equation of motion,

$$
m\ddot x + kx = 0
$$

so

$$
\boxed{
\frac{dE}{dt}=0
}
$$

Thus energy is conserved.

## 5. Interpretation in phase space

Phase space uses coordinates

$$
(x,\dot x)
$$

For

$$
x(t)=C\cos(\omega_0 t+\phi)
$$

and

$$
\dot x(t)=-C\omega_0\sin(\omega_0 t+\phi)
$$

we obtain

$$
\frac{x^2}{C^2} + \frac{\dot x^2}{\omega_0^2 C^2} = 1
$$

This is an ellipse in phase space.

So the harmonic oscillator corresponds to a closed orbit in phase space, expressing periodic motion and energy conservation.

---

# Problem 9 — Potential and conservative field

Given

$$
U(x,y)=\frac{k}{2}(x^2+y^2)
$$

## 1. Force as the gradient of the potential

For a conservative force:

$$
\vec F = -\nabla U
$$

Compute the gradient:

$$
\nabla U =
\left(
\frac{\partial U}{\partial x},
\frac{\partial U}{\partial y}
\right)
=
(kx,ky)
$$

Therefore

$$
\boxed{
\vec F(x,y)=(-kx,-ky)
}
$$

## 2. Equations of motion

Newton's second law gives

$$
m\ddot x = -kx
$$

$$
m\ddot y = -ky
$$

Thus

$$
\boxed{
m\ddot x + kx = 0,
\qquad
m\ddot y + ky = 0
}
$$

## 3. Type of motion

This is a two-dimensional isotropic harmonic oscillator.

The motions in the two directions are independent:

$$
x(t)=A_x\cos(\omega t)+B_x\sin(\omega t)
$$

$$
y(t)=A_y\cos(\omega t)+B_y\sin(\omega t)
$$

with

$$
\omega=\sqrt{\frac{k}{m}}
$$

The trajectory depends on the initial conditions:

- straight line,
- ellipse,
- circle.

A circle occurs when the amplitudes are equal and the phase shift is $\frac{\pi}{2}$.

## 4. Total energy

The total energy is

$$
\boxed{
E=
\frac{1}{2}m(\dot x^2+\dot y^2)
+
\frac{1}{2}k(x^2+y^2)
}
$$

It is constant in time.

## 5. Geometric interpretation

Since the same restoring force acts toward the origin in both directions, the particle oscillates around the equilibrium point

$$
(x,y)=(0,0)
$$

The orbit is generally an ellipse centered at the origin.

## 6. Example HTML/JS application

Save the following as `task_09_visualization.html` and open it in a browser:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>2D Harmonic Oscillator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      background: #f7f7f7;
    }
    canvas {
      background: white;
      border: 1px solid #ccc;
    }
  </style>
</head>
<body>
  <h2>2D Isotropic Harmonic Oscillator</h2>
  <p>Trajectory of a particle in the potential U(x,y) = (k/2)(x²+y²).</p>
  <canvas id="canvas" width="700" height="500"></canvas>

  <script>
    const canvas = document.getElementById("canvas");
    const ctx = canvas.getContext("2d");

    const A = 120;
    const B = 80;
    const omega = 1.2;
    const phi = Math.PI / 3;

    const cx = canvas.width / 2;
    const cy = canvas.height / 2;

    let t = 0;
    const trail = [];

    function drawAxes() {
      ctx.strokeStyle = "#999";
      ctx.lineWidth = 1;

      ctx.beginPath();
      ctx.moveTo(0, cy);
      ctx.lineTo(canvas.width, cy);
      ctx.stroke();

      ctx.beginPath();
      ctx.moveTo(cx, 0);
      ctx.lineTo(cx, canvas.height);
      ctx.stroke();
    }

    function animate() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      drawAxes();

      const x = A * Math.cos(omega * t);
      const y = B * Math.cos(omega * t + phi);

      trail.push([x, y]);
      if (trail.length > 400) trail.shift();

      ctx.beginPath();
      for (let i = 0; i < trail.length; i++) {
        const px = cx + trail[i][0];
        const py = cy - trail[i][1];
        if (i === 0) ctx.moveTo(px, py);
        else ctx.lineTo(px, py);
      }
      ctx.strokeStyle = "#0066cc";
      ctx.lineWidth = 2;
      ctx.stroke();

      ctx.beginPath();
      ctx.arc(cx + x, cy - y, 6, 0, 2 * Math.PI);
      ctx.fillStyle = "#cc0000";
      ctx.fill();

      ctx.fillStyle = "#000";
      ctx.fillText("O", cx + 5, cy - 5);

      t += 0.02;
      requestAnimationFrame(animate);
    }

    animate();
  </script>
</body>
</html>
```

---

# Problem 10 — Numerical model of a dynamical system

Consider the potential

$$
U(x)=\frac{k}{2}x^2+\lambda x^4
$$

## 1. Force

The force is

$$
F(x) = -\frac{dU}{dx}
$$

Differentiate:

$$
\frac{dU}{dx}=kx+4\lambda x^3
$$

Therefore

$$
\boxed{
F(x)= -kx - 4\lambda x^3
}
$$

## 2. Equation of motion

Newton's second law gives

$$
m\ddot x = -kx - 4\lambda x^3
$$

Thus

$$
\boxed{
m\ddot x + kx + 4\lambda x^3 = 0
}
$$

This is a nonlinear oscillator.

## 3. Numerical solution for selected parameters

A convenient example is

$$
m=1,
\qquad
k=1,
\qquad
\lambda=0.25
$$

Then the system becomes

$$
\ddot x = -x - x^3
$$

A numerical solution can be obtained from the first-order system

$$
\frac{dx}{dt}=v
$$

$$
\frac{dv}{dt}=-\frac{k}{m}x-\frac{4\lambda}{m}x^3
$$

Example Python code:

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp

m = 1.0
k = 1.0
lam = 0.25

x0 = 1.2
v0 = 0.0

def rhs(t, y):
    x, v = y
    dxdt = v
    dvdt = -(k/m) * x - (4 * lam / m) * x**3
    return [dxdt, dvdt]

t_span = (0, 40)
t_eval = np.linspace(*t_span, 4000)

sol = solve_ivp(rhs, t_span, [x0, v0], t_eval=t_eval)

t = sol.t
x = sol.y[0]
v = sol.y[1]

plt.figure(figsize=(9, 4))
plt.plot(t, x)
plt.xlabel("t")
plt.ylabel("x(t)")
plt.title("Time evolution")
plt.grid()
plt.show()

plt.figure(figsize=(6, 6))
plt.plot(x, v)
plt.xlabel("x")
plt.ylabel("v")
plt.title("Phase portrait")
plt.grid()
plt.show()
```

## 4. Effect of initial energy on the type of motion

The total energy is

$$
E=\frac{1}{2}mv^2+\frac{k}{2}x^2+\lambda x^4
$$

For

$$
\lambda > 0
$$

the potential grows strongly for large $|x|$, so the motion remains bounded for any finite energy.

As the initial energy increases:

- the oscillation amplitude increases,
- the restoring force becomes more nonlinear,
- the period depends on amplitude,
- the phase portrait remains closed, but it is no longer an ellipse.

So this is an anharmonic oscillator.

## 5. Interpretation of the visualization

- The graph of $x(t)$ shows oscillatory motion, but not perfectly sinusoidal motion.
- The phase portrait shows closed loops, confirming bounded motion.
- Compared with the harmonic oscillator, the loops become distorted because of the quartic term.

---

# Final remarks

This problem set shows the connection between:

- Newton's second law,
- work and energy,
- momentum conservation,
- damping,
- oscillations,
- numerical modeling.

A very important pattern appears repeatedly:

$$
\text{equation of motion} \quad \longrightarrow \quad \text{solution} \quad \longrightarrow \quad \text{physical interpretation}
$$

That is exactly the structure worth remembering for class discussion and exam preparation.