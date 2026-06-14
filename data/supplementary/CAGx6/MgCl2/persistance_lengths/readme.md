# Persistence Lengths (MgCl2)

Persistence lengths for rCAGx6, dCAGx6, and rCmAGx6 computed from all-atom MD simulations in 150 mM MgCl2 at 293 K and 368 K.

## Files

| File | Description |
|------|-------------|
| `persistence_values.dat` | Persistence length (mean ± s.e.m.) for all sequences and temperatures |

## Data Format

Plain text; one line per sequence/temperature combination:

```
{sequence} at {temperature}K, means = [{run1}, {run2}, {run3}]Å, average: {mean}Å, s.e.m: {sem}Å
```

Values are in angstroms (Å). Three independent replicates are reported alongside the mean and standard error of the mean.
