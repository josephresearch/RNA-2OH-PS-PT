# Figure 4 Data

All-atom MD simulation data for the modified sequence r(CmAG)6 at two temperatures (20°C / 293 K and 95°C / 368 K) in 150 mM MgCl2. Contains the same observables as the Figure 1 dataset — radius of gyration time series and Mg2+ / water solvation shell counts — for this single sequence.

## Files

| File | Observable | Sequence |
|------|-----------|----------|
| `Rg_rCmAGx6_293_150mM_500ns.dat` | Rg time series at 293 K | r(CmAG)6 |
| `Rg_rCmAGx6_368_150mM_500ns.dat` | Rg time series at 368 K | r(CmAG)6 |
| `Mg_solvation_rCmAGx6.dat` | Avg. Mg2+ ions within 5 Å of Op | r(CmAG)6 |
| `water_solvation_rCmAGx6.dat` | Avg. H2O molecules within 5 Å of Op | r(CmAG)6 |

## Data Formats

### Rg time series (`Rg_*.dat`)

Tab-separated; sampled every 0.1 ns from 100 ns to 500 ns of production simulation:

```
# step(ns), run1 rg(Å), run2 rg(Å), run3 rg(Å)
```

- **Column 1 — step (ns):** simulation time
- **Columns 2–4 — rg (Å):** radius of gyration for each of the three independent replicates

### Solvation data (`Mg_solvation_rCmAGx6.dat`, `water_solvation_rCmAGx6.dat`)

Comma-separated; one row per temperature:

```
# Nucleic Acid, temperature (K), run1, run2, run3
```

- **Column 1 — Nucleic Acid:** sequence identifier (`rCmAGx6`)
- **Column 2 — temperature (K):** 293 or 368
- **Columns 3–5:** average count of Mg2+ ions (or H2O molecules) within 5 Å of the phosphate oxygen (Op) for each replicate; encompasses the 1st and 2nd solvation shells
