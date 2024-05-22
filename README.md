# Biomarker-Guided scRNA-Seq Cancer Attractor Analysis

## Overview
This repository provides code for a biomarker-guided uncovering of potential cancer attractors given a single-cell RNA sequencing (scRNA-seq) processed count matrix. The pipeline executes biomarker-oriented clustering and ellipsoidal statistics to identify high-density regions within the data. Further, exploring gene regulatory network (GRN) stochastic dynamics allows for verifying these regions for cancer attractor candidates. The output reveals the biomarkers’ potential to identify cancer attractors, the corresponding confidence regions, and clusters’ multistability as potential sources for cancer recurrence. This framework complements the biomarkers’ investigation and their potential to define cancer attractors. Additionally, it gives essential insights concerning the underlying dynamics driving cancer progression and treatment.

## Features
- Investigate biomarkers’ potential of finding  cancer attractors
- Finding parameters conferring specified stability to a GRN dynamics
- Use of stochastic simulations to refine attractors’ identification
- Use of stochastic simulations to identify likely multistability

## Input Files

1. Gene expression data: 
   - "datapoints_seurat_BT_ALL.xlsx"
   - "datapoints_seurat_BT_S1.xlsx"
   - "datapoints_seurat_BT_S2.xlsx"
   - "datapoints_seurat_BT_S4.xlsx"
   - "datapoints_seurat_BT_S6.xlsx"
   - "datapoints_seurat_Regular.xlsx"
   
   These datasets contain gene expression data from multiple patients. The data can be obtained from the [link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE84465).

2. Activation and inhibition adjacency matrices: 
   - "act_BT_ALL_seurat.xlsx"
   - "sup_BT_ALL_seurat.xlsx"
   
   These are the activation adjacency matrices corresponding to the GRN dynamic model.

## Usage
1. **Data**: Input scRNA-seq data in a normalized count matrix format with adjacency matrices corresponding to the GRNs’ activation and inhibition interactions.
2. **Clustering**: Select the desired biomarker dimensions to identify the confidence regions to investigate the presence of cancer attractors.
3. **Attractor Inference**: Refine attractor identification using stochastic simulations. This step could be adjusted accordingly, changing the size of confidence regions, regulation functions, range of parameter investigation, and more specific technical configurations.

## Dependencies
- Wolfram Mathematica version 13.1

## Example
- The article results could be reproduced by running the notebook.

## License

This project is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](LICENSE.txt).

### License Summary

This license allows others to remix, adapt, and build upon this work non-commercially, as long as they credit the original author and license their new creations under the same terms. For more details, please visit the [license page](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Contribution
Any contributions are welcome.

## Authors
- [Marcos Vieira](https://github.com/marcosgvjunior)

## References
- The code provided in this repository is associated with an upcoming research article.

