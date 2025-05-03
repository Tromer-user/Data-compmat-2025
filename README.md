# Data-compmat-2025
# Dataset: Barrier Calculations for 2D Materials from the C2DB Database

This dataset contains computed barrier values for ionic movement in two-dimensional (2D) materials, based on structures extracted from the **Computational 2D Materials Database (C2DB)**. The barrier values were obtained using a **Hückel-type approximation** developed in our work, with values reported along different crystallographic directions.

## 📁 File

- `2D_database_barrier_oxygen.csv`: Main dataset file, where each row corresponds to a 2D material from the C2DB.

## 📊 Columns Description

| Column | Description |
|--------|-------------|
| `ind` | Index of the material in the C2DB (e.g. 9 = graphene) |
| `max_valorX` | Maximum ionic barrier in the X direction |
| `max_valorY` | Maximum ionic barrier in the Y direction |
| `max_valorZ` | Maximum ionic barrier in the diagonal XY direction |
| `media` | Average barrier value across all directions |
| `formula` | Chemical formula of the 2D material |
| `Ehull` | Energy above the convex hull (eV) |
| `HF` | Heat of formation (eV/atom) |
| `Gap` | Band gap (eV) |
| `Energy` | Total energy per unit cell (DFT-calculated) |
| `natoms` | Number of atoms in the unit cell |
| `nspecies` | Number of chemical species |
| `thickness` | Structural thickness of the 2D material (Å) |
| `uc_area` | Unit cell area (Å²) |
| `average_atomic_number` | Average atomic number of the elements in the material |
| `average_valence_number` | Average number of valence electrons per atom |
| `average_electronegativity` | Average electronegativity of the constituent atoms |

## 🔍 Example Entries

| formula | max_valorX | max_valorY | max_valorZ | media | Gap | Energy |
|---------|-------------|-------------|------------|--------|------|--------|
| Y₂Se₆   | 0.4975      | 0.6775      | 1.0825     | 0.7525 | 0.0  | -40.015 |
| Zr₂O₆   | 0.4750      | 0.1700      | 0.3700     | 0.3383 | 3.586| -65.407 |
| C₂ (graphene) | 0.6773 | 0.6930      | 0.6855     | 0.6853 | 0.0  | -18.454 |

## 🧪 Methodology Summary

- Structural and compositional data were sourced from the [C2DB](https://cmr.fysik.dtu.dk/c2db/).
- Ionic migration barriers in X, Y, and XY directions were estimated using a **Hückel-based potential energy approximation**.
- All properties like energy, gap, thickness, etc., refer to standard DFT values as available in the C2DB.

## 📎 Citation

If using this dataset, please cite the associated article (in preparation/submitted to *Computational Materials Science*) and acknowledge the C2DB project.

---

*For questions or suggestions, please contact the corresponding author or open an issue on this repository.*
