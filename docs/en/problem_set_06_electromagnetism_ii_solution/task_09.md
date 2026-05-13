## Problem 9 — Ideal vs. real transformer

### How it works

A transformer consists of two coils (primary $N_1$ turns, secondary $N_2$ turns) wound on a common ferromagnetic core. An AC current in the primary creates a time-varying magnetic flux $\Phi(t)$ in the core. By Faraday's law, this flux induces an EMF in both coils:

$$
\mathcal{E}_1 = -N_1\frac{d\Phi}{dt}, \quad \mathcal{E}_2 = -N_2\frac{d\Phi}{dt}
$$

### Ideal transformer

- No losses ($\eta = 100\%$).
- All flux is confined to the core (perfect coupling).
- Voltage ratio:

$$
\frac{U_2}{U_1} = \frac{N_2}{N_1}
$$

- Current ratio (from power conservation $U_1 I_1 = U_2 I_2$):

$$
\frac{I_2}{I_1} = \frac{N_1}{N_2}
$$

### Origin of secondary voltage

It comes from the **changing magnetic flux** in the core, induced by the primary current. No direct electrical connection between the windings is needed — the energy transfer is purely electromagnetic.

### Losses in real transformers

1. **Copper losses** ($I^2R$) — resistance of the windings.
2. **Iron losses**:
   - **Hysteresis losses** — energy lost in repeatedly magnetizing/demagnetizing the core.
   - **Eddy current losses** in the core — reduced by laminating the core.
3. **Flux leakage** — not all flux from the primary links the secondary.
4. **Magnetizing current** — needed to magnetize the core even with no load.

### Typical values

- Turns ratio: from $\sim 1:1$ (isolation transformers) to $\sim 1000:1$ (high-voltage power transformers).
- Efficiency of large power transformers: **95–99%**.
- Small consumer transformers: **70–90%**.