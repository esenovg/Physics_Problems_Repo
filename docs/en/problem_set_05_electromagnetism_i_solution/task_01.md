# Problem 1 – Potential and energy

We are given a point charge:

$$
q = 4\ \mu\mathrm{C} = 4.0 \cdot 10^{-6}\ \mathrm{C}
$$

The test charge is:

$$
q_0 = 2\ \mu\mathrm{C} = 2.0 \cdot 10^{-6}\ \mathrm{C}
$$

The electrostatic constant is:

$$
k = \frac{1}{4\pi \varepsilon_0} \approx 8.99 \cdot 10^9\ \mathrm{N\,m^2/C^2}
$$

For a point charge, the electric potential is:

$$
V(r) = k\frac{q}{r}
$$

We assume that the potential is zero at infinity:

$$
V(\infty) = 0
$$

---

## 1. Potential at distance \( r = 0.3\,\mathrm{m} \)

The formula for the electric potential of a point charge is:

$$
V(r) = k\frac{q}{r}
$$

For:

$$
r = 0.3\ \mathrm{m}
$$

we get:

$$
\begin{aligned}
V(0.3)
&= k\frac{q}{0.3} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{0.3} \\
&= \frac{3.596 \cdot 10^4}{0.3} \\
&= 1.1987 \cdot 10^5\ \mathrm{V}
\end{aligned}
$$

Therefore:

$$
\boxed{V(0.3) \approx 1.20 \cdot 10^5\ \mathrm{V}}
$$

or:

$$
\boxed{V(0.3) \approx 120\ \mathrm{kV}}
$$

---

## 2. Potential difference between \( 0.3\,\mathrm{m} \) and \( 0.6\,\mathrm{m} \)

First, calculate the potential at:

$$
r = 0.6\ \mathrm{m}
$$

Using:

$$
V(r) = k\frac{q}{r}
$$

we get:

$$
\begin{aligned}
V(0.6)
&= k\frac{q}{0.6} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{0.6} \\
&= \frac{3.596 \cdot 10^4}{0.6} \\
&= 5.993 \cdot 10^4\ \mathrm{V}
\end{aligned}
$$

Therefore:

$$
\boxed{V(0.6) \approx 5.99 \cdot 10^4\ \mathrm{V}}
$$

or:

$$
\boxed{V(0.6) \approx 59.9\ \mathrm{kV}}
$$

The potential difference for motion from \( 0.3\,\mathrm{m} \) to \( 0.6\,\mathrm{m} \) is:

$$
\Delta V = V(0.6) - V(0.3)
$$

Substituting the values:

$$
\begin{aligned}
\Delta V
&= 5.993 \cdot 10^4 - 1.1987 \cdot 10^5 \\
&= -5.993 \cdot 10^4\ \mathrm{V}
\end{aligned}
$$

Therefore:

$$
\boxed{\Delta V \approx -5.99 \cdot 10^4\ \mathrm{V}}
$$

or:

$$
\boxed{\Delta V \approx -59.9\ \mathrm{kV}}
$$

The negative sign means that the potential decreases when we move farther away from a positive point charge.

The magnitude of the potential difference is:

$$
\boxed{|\Delta V| \approx 5.99 \cdot 10^4\ \mathrm{V}}
$$

---

## 3. Work done to move the test charge

The change in electric potential energy is:

$$
\Delta U = q_0 \Delta V
$$

Substitute:

$$
q_0 = 2.0 \cdot 10^{-6}\ \mathrm{C}
$$

and:

$$
\Delta V = -5.993 \cdot 10^4\ \mathrm{V}
$$

Then:

$$
\begin{aligned}
\Delta U
&= q_0 \Delta V \\
&= \left(2.0 \cdot 10^{-6}\right)\left(-5.993 \cdot 10^4\right) \\
&= -1.1986 \cdot 10^{-1}\ \mathrm{J} \\
&\approx -0.120\ \mathrm{J}
\end{aligned}
$$

Therefore, the change in potential energy is:

$$
\boxed{\Delta U \approx -0.120\ \mathrm{J}}
$$

The work done by the electric field is the negative of the change in potential energy:

$$
W_{\mathrm{field}} = -\Delta U
$$

Therefore:

$$
\begin{aligned}
W_{\mathrm{field}}
&= -\left(-0.120\ \mathrm{J}\right) \\
&= 0.120\ \mathrm{J}
\end{aligned}
$$

So:

$$
\boxed{W_{\mathrm{field}} \approx 0.120\ \mathrm{J}}
$$

If the charge is moved slowly by an external force, then the external work is:

$$
W_{\mathrm{external}} = \Delta U
$$

Therefore:

$$
\boxed{W_{\mathrm{external}} \approx -0.120\ \mathrm{J}}
$$

This result is negative because the positive test charge naturally moves away from the positive source charge. The electric field helps the motion from \( 0.3\,\mathrm{m} \) to \( 0.6\,\mathrm{m} \).

---

## 4. Electric field intensity from the derivative of the potential

The electric field is related to the electric potential by:

$$
\vec E = -\nabla V
$$

Because the point charge has spherical symmetry, the potential depends only on the distance \( r \). Therefore:

$$
E_r = -\frac{dV}{dr}
$$

The potential of a point charge is:

$$
V(r) = k\frac{q}{r}
$$

Differentiate with respect to \( r \):

$$
\begin{aligned}
\frac{dV}{dr}
&= \frac{d}{dr}\left(k\frac{q}{r}\right) \\
&= kq\frac{d}{dr}\left(r^{-1}\right) \\
&= kq\left(-r^{-2}\right) \\
&= -k\frac{q}{r^2}
\end{aligned}
$$

Therefore:

$$
\begin{aligned}
E_r
&= -\frac{dV}{dr} \\
&= -\left(-k\frac{q}{r^2}\right) \\
&= k\frac{q}{r^2}
\end{aligned}
$$

So the electric field vector is:

$$
\boxed{\vec E(r) = k\frac{q}{r^2}\hat r}
$$

Because \( q > 0 \), the field points radially outward from the charge.

At \( r = 0.3\,\mathrm{m} \):

$$
\begin{aligned}
E(0.3)
&= k\frac{q}{(0.3)^2} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{(0.3)^2} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{0.09} \\
&= \frac{3.596 \cdot 10^4}{0.09} \\
&= 3.996 \cdot 10^5\ \mathrm{N/C}
\end{aligned}
$$

Therefore:

$$
\boxed{E(0.3) \approx 4.00 \cdot 10^5\ \mathrm{N/C}}
$$

At \( r = 0.6\,\mathrm{m} \):

$$
\begin{aligned}
E(0.6)
&= k\frac{q}{(0.6)^2} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{(0.6)^2} \\
&= 8.99 \cdot 10^9 \cdot \frac{4.0 \cdot 10^{-6}}{0.36} \\
&= \frac{3.596 \cdot 10^4}{0.36} \\
&= 9.989 \cdot 10^4\ \mathrm{N/C}
\end{aligned}
$$

Therefore:

$$
\boxed{E(0.6) \approx 9.99 \cdot 10^4\ \mathrm{N/C}}
$$

---

## 5. Comparison with Coulomb's law

From the derivative of the potential, we found:

$$
\vec E(r) = k\frac{q}{r^2}\hat r
$$

Coulomb's law gives the electric field of a point charge directly as:

$$
\vec E(r) = k\frac{q}{r^2}\hat r
$$

Therefore:

$$
\boxed{\vec E_{\mathrm{from\ potential}} = \vec E_{\mathrm{from\ Coulomb}}}
$$

The result obtained from the potential agrees exactly with Coulomb's law.

Since the charge is positive:

$$
q > 0
$$

the electric field points away from the charge:

$$
\boxed{\text{The electric field is directed radially outward.}}
$$

---

## Final answers

Potential at \( r = 0.3\,\mathrm{m} \):

$$
\boxed{V(0.3) \approx 1.20 \cdot 10^5\ \mathrm{V}}
$$

Potential at \( r = 0.6\,\mathrm{m} \):

$$
\boxed{V(0.6) \approx 5.99 \cdot 10^4\ \mathrm{V}}
$$

Potential difference from \( 0.3\,\mathrm{m} \) to \( 0.6\,\mathrm{m} \):

$$
\boxed{\Delta V \approx -5.99 \cdot 10^4\ \mathrm{V}}
$$

Change in potential energy of the test charge:

$$
\boxed{\Delta U \approx -0.120\ \mathrm{J}}
$$

Work done by the electric field:

$$
\boxed{W_{\mathrm{field}} \approx 0.120\ \mathrm{J}}
$$

External work for slow motion:

$$
\boxed{W_{\mathrm{external}} \approx -0.120\ \mathrm{J}}
$$

Electric field from the potential:

$$
\boxed{\vec E(r) = k\frac{q}{r^2}\hat r}
$$

Electric field at \( r = 0.3\,\mathrm{m} \):

$$
\boxed{E(0.3) \approx 4.00 \cdot 10^5\ \mathrm{N/C}}
$$

Electric field at \( r = 0.6\,\mathrm{m} \):

$$
\boxed{E(0.6) \approx 9.99 \cdot 10^4\ \mathrm{N/C}}
$$

The field from the derivative of the potential agrees with Coulomb's law:

$$
\boxed{\vec E_{\mathrm{from\ potential}} = \vec E_{\mathrm{from\ Coulomb}}}
$$