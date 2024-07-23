# Network-Based Data Analysis Project: Biliary Atresia Study
### Project for the class of Network-based Data Analysis QCB 2023/2024

- [Introduction](#introduction)
- [Project Overview](#project_overview)
  - [Exploratory Data Analysis (EDA)](#exploratory_data_analysis-eda)
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
   - Perform differential expression analysis to identify genes showing significant expression changes between experimental conditions with LIMMA.
   - Compare the DEGs with the most important features from the random forest model.

4. **Gene Ontology and Network Analysis:**
   - Investigating the relationship between gene signatures using the [SCUDO R library](https://www.cosbi.eu/prototypes/scudo).
   - Performing Over-Representation Analysis (ORA) with [gprofiler](https://biit.cs.ut.ee/gprofiler/gost).
   - Analyzing Protein-Protein Interaction (PPI) networks with [STRING](https://string-db.org/).
   - DAVID
   - pathfindeR
   
## Conclusion
This analysis sought to enhance the histological classification of biliary atresia (BA) by integrating machine learning with gene expression data from 47 infants diagnosed with the disease. The study involved unsupervised learning techniques, including UMAP and PAM clustering, which revealed an approximate division aligning with known molecular groups, despite some bias from sex-related probes. Various models were tested, with Random Forest outperforming LASSO due to a higher F1 score, and successfully classifying four previously unclassified samples.

Key findings include the identification of high-importance genes such as SLC24A1, ARF6, and DUSP5, which were consistent with existing literature on BA. This suggests that machine learning models can not only classify samples but also highlight potential new targets for research. Differential expression analysis identified a significant number of differentially expressed genes (DEGs) between molecular groups, indicating potential distinct disease stages and revealing patterns that could be relevant for further investigation.

Functional enrichment analysis using DAVID and gProfiler identified common terms related to collagen organization and inflammatory response across molecular groups. STRING analysis showed distinct clusters, while pathfindR highlighted terms associated with viral infections and diseases. Notably, DUSP5 emerged as a potential marker of external influence in BA, and ADRB2 could be a target for experimental treatment in early inflammatory stages.

Overall, this study demonstrates the value of combining molecular insights with advanced machine learning models to understand BA better. Future research should focus on refining models, incorporating additional data, and exploring the inflammatory aspects of the disease to uncover further details and potential therapeutic targets.
