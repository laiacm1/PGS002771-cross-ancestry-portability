# Numerical and Disease-Effect Portability of Polygenic Scores Across Ancestry Groups

This repository contains analysis code and derived outputs supporting the manuscript:

**“Distinguishing Numerical and Disease-Effect Portability of Polygenic Scores Across Ancestry Groups”**

## Overview

This study examines the distinction between numerical polygenic-score portability and cross-ancestry disease-effect portability.

The analyses distinguish between:

- **Numerical PGS displacement:** ancestry-associated changes in variant contributions to a fixed polygenic score, driven in part by differences in effect-allele frequency and score weights.
- **Cross-ancestry disease-effect differences:** differences in ancestry-specific marginal disease-effect estimates obtained from external GWAS summary statistics.

The revised study extends the original PGS002771 analysis across multiple scores, biological-support analyses, an additional disease context, and an independent phenotype-linked cohort.

## Analyses included

The repository contains analyses supporting:

1. Cross-ancestry numerical displacement of PGS002771
2. Recurrence of high-displacement variants across ancestry comparisons
3. Weight- and allele-frequency-matched permutation analysis
4. Comparison with ancestry-specific T2D effect estimates
5. Exploratory local linkage disequilibrium analysis
6. Cross-PGS comparison across four published T2D polygenic scores
7. Enrichment of recurrent high-displacement variants for T2D fine-mapping support
8. Cross-disease replication using the coronary artery disease score PGS004198
9. Independent phenotype-linked validation of PGS002771 using the Harvard Personal Genome Project

## Repository structure

### Original PGS002771 analyses

The original analysis notebook is:

`PGS002771_cross_ancestry_portability (5).ipynb`

This notebook contains the primary PGS002771 cross-ancestry analyses and figure-generation code.

### Cross-PGS T2D analysis

See:

`cross_pgs_t2d/`

This directory contains the comparison of EUR–SAS numerical displacement with standardized ancestry-specific T2D effect differences across:

- PGS002771
- PGS000036
- PGS002426
- PGS002475

### T2D fine-mapping enrichment

See:

`fine_mapping/`

This directory contains the analysis testing whether recurrent high-displacement variants overlap T2D credible-set variants from published fine-mapping results more often than comparison variants.

### CAD replication

See:

`cad_replication/`

This directory contains the cross-disease replication analysis using PGS004198 and EUR–SAS CAD effect estimates.

Primary outputs include the Spearman correlation, block-bootstrap confidence interval, leave-one-chromosome-out estimates, and secondary raw-effect comparison.

### PGP phenotype-linked validation

See:

`pgp_validation/`

This directory contains the independent phenotype-linked validation of PGS002771 using the Harvard Personal Genome Project.

Primary analyses include logistic regression of T2D status on standardized PGS002771, ROC-AUC estimation, bootstrap confidence intervals, and phenotype-label permutation testing.

Raw participant-level genotype and phenotype data are not redistributed in this repository.

## Data sources

The analyses use publicly available data from:

- **PGS Catalog:** PGS002771, PGS000036, PGS002426, PGS002475, and PGS004198
- **1000 Genomes Project Phase 3:** ancestry-specific genotype and allele-frequency data
- **Type 2 Diabetes Global Genomics Initiative:** ancestry-specific T2D GWAS summary statistics
- **Mahajan et al.:** T2D fine-mapping results
- **CARDIoGRAMplusC4D / Aragam et al.:** European-ancestry CAD GWAS summary statistics
- **Genes & Health:** South Asian CAD GWAS summary statistics
- **Harvard Personal Genome Project:** participant-level genotype and phenotype data used for independent validation

Large source genotype, GWAS, and participant-level files are not redistributed in this repository.

## Reproducibility

The repository contains analysis notebooks and derived outputs used for the final manuscript analyses.

Because several large external datasets are not redistributed here, the notebooks expect the required source or derived input files to be available locally using the file paths documented in the analysis code.

Stochastic procedures use fixed random seeds where applicable.

## Author

Laia Chandran-Moles  
Los Gatos High School  
Los Gatos, California, USA
