# Network-Based Data Analysis Project: Biliary Atresia Study
### Project for the class of Network-based Data Analysis QCB 2023/2024

- [Introduction](#introduction)
- [Project Overview](#project-overview)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Predictive Modeling](#predictive-modeling)
  - [Differential Expression Analysis](#differential-expression-analysis)
  - [Gene Ontology and Network Analysis](#gene-ontology-and-network-analysis)
- [Key R Packages](#key-r-packages)
- [Conclusion](#conclusion)

Link for the report [here](https://www.overleaf.com/project/65e5fb710b468abfd7e67ca4).

## Introduction

Welcome to the `Network-Based Data Analysis` project for the QCB 2023/2024 class. In this project, we will delve into the world of molecular profiling in biliary atresia, utilizing the dataset GSE15235 obtained from a prospective observational study conducted by [Moyer, Katie, et al.](https://link.springer.com/article/10.1186/gm154). This study aims to explore the molecular signatures associated with inflammation and fibrosis in the livers of infants diagnosed with biliary atresia.

### Project Overview

The analysis will focus on the following key aspects:

1. **Exploratory Data Analysis (EDA):**
   - Preliminary approach to analyzing data, through visualization and summary statistics (UMAP and PCA), to understand its structure, patterns, and characteristics.
   - Investigating the gene signatures that distinguish between inflammation and fibrosis.
   - Exploring potential associations between gene profiles and clinical outcomes.

2. **Predictive Modeling:**
   - Feature selection to understand the genes which most contribute to each class.
   - Utilizing prediction analysis models to classify livers into inflammation or fibrosis based on gene expression profiles.
   - Validating predictions through statistical analyses, including cross-validation on each model.

3. **Differential Expression Analysis (DEGs):**
   - Perform differential expression analysis to identify genes showing significant expression changes between experimental conditions.
   - Utilize [Enrichr](https://maayanlab.cloud/Enrichr/) to explore drug signatures and pharmacological data to investigate potential drug targets and mechanisms of action related to the observed gene expression changes.

4. **Gene Ontology and Network Analysis:**
   - Investigating the relationship between gene signatures using the [SCUDO R library](https://www.cosbi.eu/prototypes/scudo).
   - Performing Over-Representation Analysis (ORA) with [gprofiler](https://biit.cs.ut.ee/gprofiler/gost).
   - Analyzing Protein-Protein Interaction (PPI) networks with [STRING](https://string-db.org/).

### Key R Packages

- [`caret`](https://topepo.github.io/caret/): For building and evaluating predictive models.
- [`glmnet`](https://cran.r-project.org/web/packages/glmnet/index.html): For fitting feature selection (relaxed LASSO / Elastic net).
- [`GEOquery`](https://www.bioconductor.org/packages/release/bioc/html/GEOquery.html): For accessing and retrieving Gene Expression Omnibus (GEO) data.
- [`limma`](https://bioconductor.org/packages/release/bioc/html/limma.html): For linear modeling of microarray data and differential expression analysis.
- [`plotly`](https://plotly.com/r/): Interactive plotting library for creating dynamic and interactive visualizations.
- [`FactoMineR`](https://cran.r-project.org/web/packages/FactoMineR/index.html): For multivariate exploratory data analysis, including PCA and clustering.
- [`cluster`](https://cran.r-project.org/web/packages/cluster/index.html): To perform PAM (Partitioning Around Medoids) and other clustering methods.
- [`enrichR`](https://cran.r-project.org/web/packages/enrichR/index.html): For gene set enrichment analysis to identify enriched biological pathways.
- [`rScudo`](https://bioconductor.org/packages/release/bioc/html/rScudo.html): To perform SCUDO (Signature-based Clustering for Diagnostic Purposes) for classification.
- [`EnhancedVolcano`](https://bioconductor.org/packages/release/bioc/html/EnhancedVolcano.html): For volcano plots with enhanced features for visualizing differential expression results.
- [`umap`](https://cran.r-project.org/web/packages/umap/index.html): For dimensionality reduction and visualization using Uniform Manifold Approximation and Projection.
- [`gprofiler2`](https://cran.r-project.org/web/packages/gprofiler2/index.html): Tools for functional enrichment analysis and gene set analysis.
- [`tidyverse`](https://www.tidyverse.org/): A collection of R packages for data science, including ggplot2, dplyr, tidyr, readr, purrr, and tibble.

## Conclusion

By the end of this project, we aim to provide a comprehensive analysis of the biliary atresia dataset, shedding light on the potential network-based interactions underlying disease progression and clinical outcomes.
- `Work in progress...`
- `Work in progress...`
- `Work in progress...`
