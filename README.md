# BBB Permeability Predictor

A rule-based computational tool to estimate blood-brain barrier (BBB) 
permeability of small molecules, using molecular descriptors and a 
simplified CNS Multiparameter Optimization (MPO) scoring framework.

## What it does
- Computes key molecular descriptors (molecular weight, LogP, TPSA, 
  hydrogen bond donors) from SMILES strings using RDKit
- Applies a simplified CNS MPO scoring function adapted from 
  Wager et al. (2010)
- Validates the scoring approach against 12 known CNS-active and 
  non-CNS drugs

## Key finding
CNS-active drugs scored higher on average (mean ≈ 3.0) than non-CNS 
drugs (mean ≈ 2.4), but with notable overlap — highlighting the 
limitations of descriptor-based models that don't account for active 
transport mechanisms like P-glycoprotein efflux.

## Tools used
Python, RDKit, Matplotlib, Jupyter Notebook

## Files
- `bbb_permeability_project.ipynb` — full analysis notebook
- `molecules.csv` — dataset of 12 drugs with SMILES and known CNS status
- `cns_chart.png` — results visualization
