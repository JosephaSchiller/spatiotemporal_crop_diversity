# spatiotemporal_crop_diversity

## Overview
This repository provides statistical workflows and geospatial datasets that explore crop diversity across Brandenburg, Germany (2011–2020).  
It includes R scripts for **Principal Component Analysis (PCA)** and **regression modelling**, as well as a GIS dataset with the resulting crop diversity proxies.  

The GIS dataset is intended for reuse in spatial analyses and is accompanied by metadata.

---

## Repository Contents

### 🔬 Analysis scripts
- **`PCA.Rmd`**  
  An R Markdown script that performs a Principal Component Analysis (PCA) on spatial and temporal crop diversity indices (each measured as Richness, Shannon’s diversity, Shannon’s evenness).  
  The resulting components are proxies for overall and spatio-temporal diversity.

- **`Regression_models.Rmd`**  
  An R Markdown script that fits and evaluates regression models using the PCA results as response variables.  
  This script illustrates how the PCA-derived proxies can be used in explanatory analyses.

### 🌍 GIS dataset
The dataset is provided as an **Shapefile**, which consists of multiple linked files:  

- **`crop_diversity.shp`** – main geometry file containing the grid cells  
- **`crop_diversity.dbf`** – attribute table with variable values (PC1, PC2, grid ID)  
- **`crop_diversity.prj`** – coordinate reference system information (likely EPSG:3035, ETRS89 / LAEA Europe)  
- **`crop_diversity.shx`** – spatial index for fast lookups  

Together, these files form the shapefile dataset with PCA-derived proxies of crop diversity aggregated on a 10 × 10 km grid.

### 🗂 Metadata
- **`metadata.yaml`**  
  A machine- and human-readable metadata file describing the dataset’s scope, variables, geographic coverage, temporal coverage, provenance, and license.  

### 📖 Documentation
- **`README.md`**  
  The file you are currently reading. Provides repository overview, file descriptions, and licensing information.

---

## Citation
If you use this repository or dataset, please cite:  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17084000.svg)](https://doi.org/10.5281/zenodo.17084000) 

---

## License
This repository and dataset are released under the **Creative Commons Attribution 4.0 International (CC-BY-4.0)** license.  
You are free to share and adapt the materials, provided appropriate credit is given.

---

## Contact
For questions or collaborations, please contact:  
**Josepha Schiller** – *Leibniz-Zentrum für Agrarlandschaftsforschung (ZALF) e.V.*  
📧 josepha.schiller@zalf.de
