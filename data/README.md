# Lab data

This folder is where **your own measured solidification data** goes. Notebook 02
(`notebooks/02_equilibrium_vs_scheil_solidification.ipynb`, section
**"✋ YOUR LAB DATA GOES HERE ✋"**) reads it and compares it with the CALPHAD
equilibrium and Scheil predictions. Nothing here is real data yet; until you add
files the notebook just prints "no data found" and skips the comparison.

Use any of the three formats — you don't need all of them. Blank templates with
the exact column names are in [`templates/`](templates/). Lines starting with `#`
are treated as comments.

| Format | Create this file | Columns |
|---|---|---|
| A. Arrest temperatures | `data/my_arrest_temperatures.csv` | `alloy_label, wt_pct_zn, liquidus_C, final_arrest_C, notes` |
| B. Fraction solid vs. T | `data/my_fraction_solid.csv` | `alloy_label, wt_pct_zn, temperature_C, fraction_solid` |
| C. Raw cooling curves | `data/cooling_curves/<run>.csv` (one per run) | `time_s, temperature_C` |

For format C, also add an entry for each file to `COOLING_CURVES` in the first
cell of the lab-data section of Notebook 02.

**Units:** temperature in °C, time in seconds, composition in **wt.% Zn**
(use the measured composition if you have a chemical analysis).
