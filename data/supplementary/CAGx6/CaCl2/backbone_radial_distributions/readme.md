# Backbone Radial Distribution Functions (CaCl2)

Radial distribution functions (RDFs) of Ca2+ ions and water molecules relative to the phosphate backbone oxygen (Op), computed from all-atom MD simulations in 150 mM CaCl2. Covers three sequences at two temperatures with three independent replicates each.

## File Naming Convention

```
{probe}_Op_{sequence}_{run}_{temperature}.dat
```

| Field | Values | Description |
|-------|--------|-------------|
| `probe` | `Ca`, `Water` | Ca2+ ion or water molecule |
| `Op` | `Op` | Phosphate backbone oxygen (reference site) |
| `sequence` | `rCAGx6`, `dCAGx6`, `rCmAGx6` | RNA, DNA, or modified nucleic acid sequence |
| `run` | `run1`, `run2`, `run3` | Independent simulation replicate |
| `temperature` | `293K`, `368K` | Simulation temperature |

## Data Format

Two-column comma-separated values:

```
# Op-Ca2+ distance r (Å), g(r)     # for Ca files
# Op-H2O distance r (Å), g(r)      # for Water files
```

- **Column 1 — r (Å):** center-to-center distance between Op and the probe
- **Column 2 — g(r):** radial distribution function
