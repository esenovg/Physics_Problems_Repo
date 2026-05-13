## Problem 7 — Loop pulled into a $B$ field region

**Given:** $a=0.20\ \mathrm{m}$, $b=0.10\ \mathrm{m}$, $B=0.60\ \mathrm{T}$, $R=0.40\ \Omega$, $v=1.5\ \mathrm{m/s}$.

Assume the loop moves along the $a$-direction; $b$ is the side perpendicular to the motion (the side that "crosses" the field boundary).

### 1. Flux during entry

Let $x(t)=vt$ be the length of the loop already inside the field. Then:

$$
\Phi(t) = B\cdot b\cdot x(t) = B\,b\,v\,t
$$

### 2. EMF and current

$$
\mathcal{E} = -\frac{d\Phi}{dt} = -Bbv
$$

The magnitude:

$$
|\mathcal{E}| = Bbv = 0.60\cdot 0.10\cdot 1.5 = 0.090\ \mathrm{V}
$$

$$
I = \frac{|\mathcal{E}|}{R} = \frac{Bbv}{R} = \frac{0.090}{0.40} = 0.225\ \mathrm{A}
$$

### 3. Braking force

The current-carrying side inside the field experiences a force $F=BIb$:

$$
\boxed{F(v) = BIb = \frac{B^2 b^2}{R}\,v}
$$

Numerically:

$$
F = \frac{(0.60)^2(0.10)^2}{0.40}\cdot 1.5 = \frac{0.0036}{0.40}\cdot 1.5 = 0.0135\ \mathrm{N}
$$

### 4. Mechanical power vs. Joule heat

Mechanical power to maintain constant $v$:

$$
P_{\text{mech}} = Fv = \frac{B^2b^2v^2}{R}
$$

Joule heat:

$$
P_{\text{Joule}} = I^2 R = \left(\frac{Bbv}{R}\right)^2 R = \frac{B^2 b^2 v^2}{R}
$$

Therefore $P_{\text{mech}} = P_{\text{Joule}}$ — energy conservation confirmed.

Numerically: $P = 0.0135\cdot 1.5 \approx 0.0203\ \mathrm{W}$.

### 5. When the loop is fully inside

Once the entire loop is in the uniform field, the flux $\Phi = B\cdot a\cdot b$ is **constant**. Then:

$$
\mathcal{E} = -\frac{d\Phi}{dt} = 0 \quad\Longrightarrow\quad I = 0
$$

No EMF, no current, no braking force — the loop moves freely.