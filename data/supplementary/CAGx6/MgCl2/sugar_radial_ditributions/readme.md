# Sugar Radial Distribution Functions (MgCl2)

Radial distribution functions (RDFs) of Mg2+ ions relative to the sugar oxygen (O2'/H2') of nucleic acids, computed from all-atom MD simulations in 150 mM MgCl2. Covers three sequences at two temperatures with three independent replicates each.

## File Naming Convention

```
Mg_sugar_{sequence}_{run}_{temperature}.dat
```

| Field | Values | Description |
|-------|--------|-------------|
| `sequence` | `rCAGx6`, `dCAGx6`, `rCmAGx6` | RNA, DNA, or modified nucleic acid sequence |
| `run` | `run1`, `run2`, `run3` | Independent simulation replicate |
| `temperature` | `293K`, `368K` | Simulation temperature |

## Data Format

Two-column comma-separated values:

```
# O2'/H2'-Mg2+ distance r (Å), g(r)
```

- **Column 1 — r (Å):** center-to-center distance between the sugar oxygen (O2' for RNA, H2' for DNA) and Mg2+
- **Column 2 — g(r):** radial distribution function
