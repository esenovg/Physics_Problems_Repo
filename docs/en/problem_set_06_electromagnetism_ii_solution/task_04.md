## Problem 4 — Rotating loop (induction)

A loop of area $S$, $N$ turns, rotates with angular velocity $\omega$ about an axis perpendicular to $\vec{B}$.

### 1. Magnetic flux $\Phi(t)$

The angle between $\hat{n}$ and $\vec{B}$ is $\theta(t)=\omega t$ (taking $\theta(0)=0$):

$$
\boxed{\Phi(t) = N\,B\,S\cos(\omega t)}
$$

### 2. EMF $\mathcal{E}(t)$

By Faraday's law:

$$
\mathcal{E}(t) = -\frac{d\Phi}{dt} = N B S\,\omega\sin(\omega t)
$$

### 3. Amplitude $\mathcal{E}_0$

$$
\boxed{\mathcal{E}_0 = N B S \omega}
$$

### 4. Dependence on $\omega$

The amplitude is **linear in $\omega$** — doubling the rotation speed doubles the peak EMF.

### 5. Interpretation

As the loop rotates, the flux through it changes sinusoidally. By Faraday's law, a changing flux induces an EMF — this is exactly the **principle of an AC generator**. Mechanical rotation energy is converted into electrical energy through the changing flux.

---

## Problem 5 — Induction in a moving rod

**Given:** $L=0.25\ \mathrm{m}$, $v=4\ \mathrm{m/s}$, $B=0.6\ \mathrm{T}$.

### 1. EMF $\mathcal{E}$

For a rod moving perpendicular to $\vec{B}$:

$$
\mathcal{E} = BLv = 0.6\cdot 0.25\cdot 4 = 0.60\ \mathrm{V}
$$

**Physical reasoning:** Free charges in the rod feel a magnetic force $\vec{F}=q\vec{v}\times\vec{B}$ that pushes positive charges to one end. Charges accumulate until the resulting electric field cancels the magnetic force; the potential difference between the ends is exactly $BLv$.

### 2. Potential difference

In an open circuit (no current flows), the potential difference equals the EMF:

$$
U = \mathcal{E} = 0.60\ \mathrm{V}
$$

### 3. Non-perpendicular motion

Only the velocity component perpendicular to $\vec{B}$ matters:

$$
\mathcal{E} = BLv\sin\phi
$$

where $\phi$ is the angle between $\vec{v}$ and $\vec{B}$. If $\vec{v}\parallel\vec{B}$, then $\mathcal{E}=0$.

### 4. Dependence on $L$

The EMF is **directly proportional to $L$**: a longer rod separates charges over a greater distance, producing a higher potential difference.