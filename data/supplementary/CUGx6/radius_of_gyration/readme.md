# Radius of Gyration — r(CUG)6

Radius of gyration (Rg) time series for r(CUG)6 at two temperatures in 150 mM MgCl2.

## File Naming Convention

```
Rg_rCUGx6_{temperature}_150mM_500ns.dat
```

| Field | Values | Description |
|-------|--------|-------------|
| `temperature` | `293`, `368` | Simulation temperature (K) |

## Data Format

Tab-separated; sampled every 0.1 ns from 100 ns to 500 ns of production simulation:

```
# step(ns), run1 rg(Å), run2 rg(Å), run3 rg(Å)
```

- **Column 1 — step (ns):** simulation time
- **Columns 2–4 — rg (Å):** radius of gyration for each of the three independent replicates
