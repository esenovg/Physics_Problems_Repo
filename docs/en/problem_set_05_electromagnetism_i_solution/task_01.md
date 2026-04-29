# Problem 1 – Potential and energy

We consider a point charge

$$
q = 4\ \mu\mathrm{C} = 4.0 \cdot 10^{-6}\ \mathrm{C}.
$$

The test charge is

$$
q_0 = 2\ \mu\mathrm{C} = 2.0 \cdot 10^{-6}\ \mathrm{C}.
$$

We use the electrostatic constant

$$
k = \frac{1}{4\pi \varepsilon_0}
\approx 8.99 \cdot 10^9\ \mathrm{N\,m^2/C^2}.
$$

For a point charge, the electric potential at distance $$r$$ is

$$
V(r) = k \frac{q}{r}.
$$

The zero of potential is assumed to be at infinity.

---

## 1. Potential at $$r = 0.3\,\mathrm{m}$$

We substitute

$$
r = 0.3\ \mathrm{m}.
$$

Therefore,

$$
V(0.3) = k \frac{q}{0.3}
$$

Substituting numerical values gives

$$
V(0.3) = 8.99 \cdot 10^9
\cdot
\frac{4.0 \cdot 10^{-6}}{0.3}.
$$

First calculate the numerator:

$$
8.99 \cdot 10^9 \cdot 4.0 \cdot 10^{-6} =
3.596 \cdot 10^4.
$$

So

$$
V(0.3) =
\frac{3.596 \cdot 10^4}{0.3} =
1.1987 \cdot 10^5\ \mathrm{V}.
$$

Thus,

$$
\boxed{
V(0.3) \approx 1.20 \cdot 10^5\ \mathrm{V}
}
$$

or approximately

$$
\boxed{
V(0.3) \approx 120\ \mathrm{kV}.
}
$$

---

## 2. Potential difference between $$0.3\,\mathrm{m}$$ and $$0.6\,\mathrm{m}$$

We calculate the potential at

$$
r = 0.6\ \mathrm{m}.
$$

Using

$$
V(r) = k \frac{q}{r},
$$

we get

$$
V(0.6) =
8.99 \cdot 10^9
\cdot
\frac{4.0 \cdot 10^{-6}}{0.6}.
$$

Therefore,

$$
V(0.6) =
\frac{3.596 \cdot 10^4}{0.6} =
5.993 \cdot 10^4\ \mathrm{V}.
$$

So

$$
\boxed{
V(0.6) \approx 5.99 \cdot 10^4\ \mathrm{V}
}
$$

or

$$
\boxed{
V(0.6) \approx 59.9\ \mathrm{kV}.
}
$$

The potential difference from $$0.3\,\mathrm{m}$$ to $$0.6\,\mathrm{m}$$ is

$$
\Delta V =
V(0.6) - V(0.3).
$$

Substituting values,

$$
\Delta V =
5.993 \cdot 10^4 -
1.1987 \cdot 10^5.
$$

Thus,

$$
\Delta V =
-5.993 \cdot 10^4\ \mathrm{V}.
$$

Therefore,

$$
\boxed{
\Delta V = V(0.6) - V(0.3)
\approx -5.99 \cdot 10^4\ \mathrm{V}
}
$$

or

$$
\boxed{
\Delta V \approx -59.9\ \mathrm{kV}.
}
$$

The negative sign means that the potential decreases when we move farther away from the positive point charge.

If we ask for the magnitude of the potential difference, then

$$
\boxed{
|\Delta V| \approx 5.99 \cdot 10^4\ \mathrm{V}.
}
$$

---

## 3. Work done to move a test charge $$q_0 = 2\,\mu\mathrm{C}$$

The change in electric potential energy is

$$
\Delta U = q_0 \Delta V.
$$

Using

$$
q_0 = 2.0 \cdot 10^{-6}\ \mathrm{C}
$$

and

$$
\Delta V = -5.993 \cdot 10^4\ \mathrm{V},
$$

we get

$$
\Delta U =
2.0 \cdot 10^{-6}
\cdot
\left(-5.993 \cdot 10^4\right).
$$

Therefore,

$$
\Delta U =
-1.1986 \cdot 10^{-1}\ \mathrm{J}.
$$

So

$$
\boxed{
\Delta U \approx -0.120\ \mathrm{J}.
}
$$

This is the change in potential energy when the positive test charge moves from

$$
0.3\ \mathrm{m}
$$

to

$$
0.6\ \mathrm{m}.
$$

The work done by the electric field is the negative of the change in potential energy:

$$
W_{\mathrm{field}} = -\Delta U.
$$

Thus,

$$
W_{\mathrm{field}}
=
0.120\ \mathrm{J}.
$$

So the electric field does positive work:

$$
\boxed{
W_{\mathrm{field}} \approx 0.120\ \mathrm{J}.
}
$$

If the charge is moved slowly by an external force, then the external work is

$$
W_{\mathrm{external}} = \Delta U.
$$

Therefore,

$$
\boxed{
W_{\mathrm{external}} \approx -0.120\ \mathrm{J}.
}
$$

The external work is negative because the positive test charge naturally moves away from the positive source charge.

---

## 4. Electric field intensity from the derivative of the potential

The electric field is related to the potential by

$$
\vec E = - \nabla V.
$$

Because this problem is spherically symmetric, the potential depends only on $$r$$, so

$$
E_r = - \frac{dV}{dr}.
$$

We know that

$$
V(r) = k \frac{q}{r}.
$$

Differentiate with respect to $$r:$$

$$
\frac{dV}{dr} =
\frac{d}{dr}
\left(
k \frac{q}{r}
\right).
$$

Since

$$
\frac{d}{dr}
\left(
\frac{1}{r}
\right) =
-\frac{1}{r^2},
$$

we obtain

$$
\frac{dV}{dr} =
-k \frac{q}{r^2}.
$$

Therefore,

$$
E_r =
-\frac{dV}{dr} =
-\left(
-k \frac{q}{r^2}
\right).
$$

So

$$
E_r = k \frac{q}{r^2}.
$$

Thus, the electric field vector is

$$
\boxed{
\vec E(r) =
k \frac{q}{r^2}\hat r.
}
$$

At

$$
r = 0.3\ \mathrm{m},
$$

we have

$$
E(0.3) =
8.99 \cdot 10^9
\cdot
\frac{4.0 \cdot 10^{-6}}{(0.3)^2}.
$$

Since

$$
(0.3)^2 = 0.09,
$$

we get

$$
E(0.3) =
\frac{3.596 \cdot 10^4}{0.09}.
$$

Therefore,

$$
E(0.3) =
3.996 \cdot 10^5\ \mathrm{N/C}.
$$

So

$$
\boxed{
E(0.3)
\approx
4.00 \cdot 10^5\ \mathrm{N/C}.
}
$$

At

$$
r = 0.6\ \mathrm{m},
$$

we have

$$
E(0.6) =
8.99 \cdot 10^9
\cdot
\frac{4.0 \cdot 10^{-6}}{(0.6)^2}.
$$

Since

$$
(0.6)^2 = 0.36,
$$

we get

$$
E(0.6) =
\frac{3.596 \cdot 10^4}{0.36}.
$$

Therefore,

$$
E(0.6) =
9.989 \cdot 10^4\ \mathrm{N/C}.
$$

So

$$
\boxed{
E(0.6)
\approx
9.99 \cdot 10^4\ \mathrm{N/C}.
}
$$

---

## 5. Comparison with Coulomb's law

Coulomb's law gives the electric field of a point charge directly as

$$
\vec E(r) =
k \frac{q}{r^2}\hat r.
$$

From the potential, we derived

$$
\vec E(r) =
-\nabla V =
k \frac{q}{r^2}\hat r.
$$

These two results are identical:

$$
\boxed{
\vec E_{\mathrm{from\ potential}} =
\vec E_{\mathrm{from\ Coulomb}}
}
$$

Therefore, the electric field obtained from the derivative of the potential agrees with Coulomb's law.

Because the charge is positive,

$$
q > 0,
$$

the electric field points radially outward from the charge.

---

## Final answers

The potential at $$0.3\,\mathrm{m}$$ is

$$
\boxed{
V(0.3) \approx 1.20 \cdot 10^5\ \mathrm{V}.
}
$$

The potential difference for motion from $$0.3\,\mathrm{m}$$ to $$0.6\,\mathrm{m}$$ is

$$
\boxed{
\Delta V \approx -5.99 \cdot 10^4\ \mathrm{V}.
}
$$

The work done by the electric field is

$$
\boxed{
W_{\mathrm{field}} \approx 0.120\ \mathrm{J}.
}
$$

The external work for slow motion is

$$
\boxed{
W_{\mathrm{external}} \approx -0.120\ \mathrm{J}.
}
$$

The electric field from the derivative of the potential is

$$
\boxed{
\vec E(r) =
k \frac{q}{r^2}\hat r.
}
$$

At $$r = 0.3\,\mathrm{m}$$,

$$
\boxed{
E(0.3)
\approx
4.00 \cdot 10^5\ \mathrm{N/C}.
}
$$

This agrees with Coulomb's law.