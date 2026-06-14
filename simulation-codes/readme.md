# Simulation Codes

Example input files for reproducing the all-atom and coarse-grained simulations described in the manuscript.

## All-Atom Simulations (`all-atom_293K/`)

Production run inputs for d(CAG)6, r(CAG)6, and r(CmAG)6 in 150 mM MgCl2 at 293 K. Each subfolder runs a 20 ns production segment continuing from the main simulations.

### Folder structure

```
all-atom_293K/
├── dCAGx6/
│   ├── production.mdp       # GROMACS run parameters
│   ├── input.gro            # Starting coordinates
│   ├── topol.top            # Topology
│   ├── index.ndx            # Index groups
│   ├── production_example.log
│   └── toppar/
│       ├── forcefield.itp
│       ├── DNAA.itp         # DNA nucleotide parameters
│       ├── MG.itp
│       ├── CLA.itp
│       └── TIP3.itp
├── rCAGx6/
│   ├── production.mdp
│   ├── input.gro
│   ├── topol.top
│   ├── index.ndx
│   └── toppar/
│       ├── forcefield.itp
│       ├── RNAA.itp         # RNA nucleotide parameters
│       ├── MG.itp
│       ├── CLA.itp
│       └── TIP3.itp
└── rCmAGx6/
    ├── production.mdp
    ├── input.gro
    ├── topol.top
    ├── index.ndx
    └── toppar/
        ├── forcefield.itp
        ├── RNAA.itp         # Modified RNA nucleotide parameters
        ├── MG.itp
        ├── CLA.itp
        └── TIP3.itp
```

### Running

Tested with GROMACS 2023.3 on a GPU:

```sh
gmx_gpu grompp -f production.mdp -o input.tpr -c input.gro -p topol.top -n index.ndx
gmx_gpu mdrun -ntomp 4 -v -deffnm production
```

---

## Coarse-Grained Simulations (`coarse-grained/`)

Example input for a minimal coarse-grained condensate simulation with bending stiffness κ = 1.

### Files

| File | Description |
|------|-------------|
| `lmp.in` | LAMMPS input script |
| `config_kappa_1.data` | Initial configuration for κ = 1 |

### Running

Tested with LAMMPS (23 Jun 2022) on 4 CPUs:

```sh
mpirun -np 4 lmp -in lmp.in
```
