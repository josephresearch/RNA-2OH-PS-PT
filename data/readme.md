# Data

Processed simulation data for reproducing all figures in the manuscript and supplementary information.

## Structure

```
data/
├── main_text/
│   ├── Figure1/    # Rg and solvation data for r(CAG)6 and d(CAG)6
│   └── Figure4/    # Rg and solvation data for r(CmAG)6
└── supplementary/
    ├── CAGx6/
    │   ├── MgCl2/
    │   │   ├── backbone_radial_distributions/   # Mg2+ and water RDFs vs. backbone Op
    │   │   ├── sugar_radial_ditributions/       # Mg2+ RDFs vs. sugar O2'/H2'
    │   │   └── persistance_lengths/             # Persistence lengths for all sequences
    │   └── CaCl2/
    │       └── backbone_radial_distributions/   # Ca2+ and water RDFs vs. backbone Op
    ├── CAGx10/
    │   ├── radial_distributions/                # Mg2+ and water RDFs for d/r(CAG)10
    │   └── radius_of_gyration/                  # Rg time series for d/r(CAG)10
    ├── CUGx6/
    │   └── radius_of_gyration/                  # Rg time series for r(CUG)6
    └── coarse-grained_order_parameters/         # S, A, N vs. stiffness κ
```

Each subdirectory contains a `readme.md` describing the files and data format.
