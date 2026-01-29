# RNA-seq ER Stress Analysis (HSPA5 / GRP78)
## Purpose
This repository contains a reproducible RNA-seq analysis workflow to
quantify and compare **HSPA5 (GRP78)** and other **ER stress genes**
across treatment conditions using public datasets.

## Biological context
HSPA5 (GRP78) is a central regulator of the endoplasmic reticulum (ER)
stress response. RNA-seq provides a transcriptional layer that complements
protein-level and functional assays.

## Data source
Public RNA-seq dataset from GEO:

- **GEO accession**: GSE315549
- **Organism**: Homo sapiens
- **Model**: AML cell line
- **Conditions**: DMSO, ABT (Venetoclax), ELI (Eliglustat), Combination

Raw data are not stored in this repository.
Expression matrices are downloaded directly from GEO.

## Workflow overview
1. Load GEO RNA-seq expression matrix (FPKM)
2. Extract genes of interest (HSPA5, XBP1, ATF4, DDIT3)
3. Log2-normalize expression values
4. Aggregate biological replicates (mean ± SD)
5. Visualize results (barplots and heatmap)

## Outputs
- Barplots of gene expression across treatments
- ER stress gene heatmap (Z-score, visualization only)

## Disclaimer
This analysis is provided as a **proof-of-concept** using public data
to demonstrate workflow feasibility and expected outputs.
