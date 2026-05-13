## Problem 8 — Self-induction (RL circuit)

**Given:** $L=0.20\ \mathrm{H}$, $R=5.0\ \Omega$, $U=12\ \mathrm{V}$.

### 1. Steady current $I_0$

In the steady state, $dI/dt=0$, so the inductor acts as a wire:

$$
I_0 = \frac{U}{R} = \frac{12}{5.0} = 2.4\ \mathrm{A}
$$

### 2. After disconnection: $I(t)$, $\tau$, $U_L(t)$

With the source removed, Kirchhoff's voltage law gives:

$$
L\frac{dI}{dt} + RI = 0
$$

Solving this first-order ODE:

$$
I(t) = I_0\, e^{-t/\tau}, \quad \tau = \frac{L}{R} = \frac{0.20}{5.0} = 0.040\ \mathrm{s} = 40\ \mathrm{ms}
$$

Voltage across the coil:

$$
U_L(t) = L\frac{dI}{dt} = -\frac{L I_0}{\tau}e^{-t/\tau} = -R I_0 e^{-t/\tau}
$$

At $t=0^+$: $|U_L| = R I_0 = 12\ \mathrm{V}$.

### 3. Energy stored before disconnection

$$
W = \frac{1}{2}LI_0^2 = \frac{1}{2}\cdot 0.20\cdot(2.4)^2 = 0.576\ \mathrm{J}
$$

### 4. Conversion to Joule heat

Total energy dissipated in $R$:

$$
W_R = \int_0^\infty I^2(t)\,R\,dt = \int_0^\infty I_0^2 e^{-2t/\tau} R\,dt = I_0^2 R\cdot\frac{\tau}{2}
$$

$$
W_R = I_0^2 R\cdot\frac{L}{2R} = \frac{1}{2}L I_0^2 = W \quad\checkmark
$$

All magnetic-field energy is converted into Joule heat.

### 5. Why does an overvoltage appear when disconnecting?

When the circuit is broken suddenly, the inductor tries to **maintain the current** (Lenz's law applied to itself). To do so, it generates a very large EMF:

$$
U_L = -L\frac{dI}{dt}
$$

If the current drops to zero almost instantly, $dI/dt$ is huge, and the voltage can spike to thousands of volts — often producing a visible spark or damaging the switch. This is why inductive loads need protective diodes or snubber circuits.