# Systems Biology Project 3: Spatial Proteomics

University of Warsaw — 3rd year Bioinformatics, 2025/2026

## Overview

Analysis of a spatial proteomics dataset acquired with Imaging Mass Cytometry (IMC) from the IMMUcan consortium. The dataset contains 253 433 single cells profiled for 40 protein markers across 132 tissue images and 5 cancer indications (HN, GI, THOR, BREAS, GU).

## Setup

```bash
conda create -n biosys_env python=3.10
conda activate biosys_env
pip install anndata squidpy numpy pandas matplotlib seaborn scipy scikit-learn
```

## Data

Download the data files from the [course Google Drive](https://drive.google.com/drive/folders/1pLrAb0Hy6kudQ-BHZ1w_afq18Z9eu_RE) and place them in a `data/` subdirectory:

```
data/
  train_adata.h5ad   # 253 433 cells, 132 images
  test_adata.h5ad    #  89 803 cells,  47 images
```

Data files are excluded from this repository (see `.gitignore`).

## Tasks

| Task | Description |
|------|-------------|
| 1 | Dataset overview |
| 2 | Marker expression distributions |
| 3 | Tumour burden and indication clustering |
| 4 | Spatial tissue map with marker overlay |
| 5 | Neighbourhood enrichment (Squidpy) |
| 6 | Immune composition around Tumour cells |
| 7 | Tumour subclustering with model selection |
| 8 | Biological interpretation of subclusters |
| 9 | Cross-cohort validation |

## Running

```bash
jupyter notebook SpatialProteomics.ipynb
```
