# All-Atom Radial Distribution Functions

Radial distribution functions (RDFs) of Mg2+ ions and water molecules relative to the phosphate backbone oxygen (Op) of nucleic acids, computed from all-atom molecular dynamics simulations. Files cover three nucleic acid sequences at two temperatures with three independent replicates each.

## File Naming Convention

```
{probe}_Op_{sequence}_{run}_{temperature}.dat
```

| Field | Values | Description |
|-------|--------|-------------|
| `probe` | `Mg`, `Water` | Mg2+ ion or water molecule |
| `Op` | `Op` | Phosphate backbone oxygen (reference site) |
| `sequence` | `rCAGx6`, `dCAGx6`, `rCmAGx6` | RNA, DNA, or modified nucleic acid sequence |
| `run` | `run1`, `run2`, `run3` | Independent simulation replicate |
| `temperature` | `293K`, `368K` | Simulation temperature |

## Data Format

Two-column comma-separated values (no header row beyond the comment line):

```
# Op-Mg2+ distance r (Å), g(r)     # for Mg files
# Op-H2O distance r (Å), g(r)      # for Water files
```

- **Column 1 — r (Å):** center-to-center distance between Op and the probe, in angstroms
- **Column 2 — g(r):** radial distribution function (pair correlation function)

