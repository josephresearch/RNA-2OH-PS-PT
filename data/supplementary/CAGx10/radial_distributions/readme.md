# Radial Distribution Functions — d/r(CAG)10

Radial distribution functions (RDFs) of Mg2+ ions and water molecules relative to the phosphate backbone oxygen (Op) for d(CAG)10 and r(CAG)10, averaged across replicates.

## File Naming Convention

```
{nucleic_acid}_OP_{probe}_RDF_{temperature}.dat
```

| Field | Values | Description |
|-------|--------|-------------|
| `nucleic_acid` | `dna`, `rna` | d(CAG)10 or r(CAG)10 |
| `probe` | `MG`, `water` | Mg2+ ion or water molecule |
| `temperature` | `293K`, `368K` | Simulation temperature |

## Data Format

Three-column comma-separated values:

```
# distance (Å), g(r), err
```

- **Column 1 — distance (Å):** center-to-center distance between Op and the probe
- **Column 2 — g(r):** mean radial distribution function averaged over replicates
- **Column 3 — err:** standard error of the mean across replicates
