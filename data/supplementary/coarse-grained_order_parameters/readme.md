# Coarse-Grained Order Parameters

Order parameters characterizing the condensate phase behavior from minimal coarse-grained model simulations, as a function of chain stiffness (κ).

## Files

| File | Description |
|------|-------------|
| `S_order.dat` | Orientational orderness S vs. κ |
| `A_anisotropy.dat` | Relative shape anisotropy A vs. κ |
| `N_neighbors.dat` | Number of interchain crosslinks N vs. κ |

## Data Format

All three files share the same three-column format:

```
# stiffness, value, standard_deviation
```

- **Column 1 — stiffness (κ):** dimensionless stiffness parameter (values: 0, 1, 2, 4)
- **Column 2 — value:** mean of the order parameter measured from simulations
- **Column 3 — standard_deviation:** standard deviation from simulations

