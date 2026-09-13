# Cross-Ancestry Portability of PGS002771

This repository contains analysis code supporting the manuscript:

**“Distinguishing Numerical and Disease-Effect Portability of a Type 2 Diabetes Polygenic Score Across Ancestry Groups”**

## Overview

This study examines the cross-ancestry portability of the European-derived type 2 diabetes polygenic score PGS002771.

The analyses distinguish between:

- **Numerical PGS displacement:** changes in the numerical contribution of variants across ancestry groups due to differences in effect-allele frequency.
- **Cross-ancestry T2D effect differences:** differences in ancestry-specific T2D effect estimates from external GWAS summary statistics.

The repository reproduces the final variant-level analyses reported in the manuscript, including:

1. Cross-ancestry numerical displacement
2. Recurrence of high-displacement variants across ancestry comparisons
3. Weight- and allele-frequency-matched permutation analysis
4. Comparison with ancestry-specific T2D effect estimates
5. Prediction of large cross-ancestry effect differences
6. Exploratory local linkage disequilibrium analysis
7. Final manuscript figures and numerical result checks

## Analysis notebook

`PGS002771_cross_ancestry_portability (5).ipynb`

The notebook contains the final analysis and figure-generation code.

## Data sources

The analyses use publicly available data from:

- **PGS Catalog:** PGS002771
- **1000 Genomes Project Phase 3:** ancestry-specific genotype and allele-frequency data
- **T2D Global Genomics Initiative (T2DGGI):** ancestry-specific type 2 diabetes GWAS summary statistics

Large source genotype and GWAS files are not redistributed in this repository.

## Reproducibility

The notebook records the software environment used for the final analyses and uses a fixed random seed for stochastic procedures.

Because large external datasets are not redistributed here, the notebook expects the required derived input files to be available locally using the directory structure documented in the notebook.

## Author

Laia Chandran-Moles  
Los Gatos High School  
Los Gatos, California, USA
