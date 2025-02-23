# K-means-clustering


This repository contains an R Markdown script for performing K-means clustering on gene expression data. The script includes steps for data loading, preprocessing, clustering, visualization, and functional enrichment analysis using Gene Ontology (GO).


The script performs the following tasks:

1. Data Load and Preprocessing:
   - Loads gene expression data from an Excel file.
   - Converts the data to a matrix and applies a log2 transformation for better visualization.

2. K-means Clustering:
   - Uses the Elbow Method to determine the optimal number of clusters.
   - Performs K-means clustering on the log-transformed data.

3. Visualization:
   - Generates a heatmap of the log-transformed TPM values.
   - Visualizes the clustering results using Principal Component Analysis (PCA).

4. Gene Ontology (GO) Enrichment Analysis:
   - Converts gene symbols to Entrez IDs.
   - Performs GO enrichment analysis for each cluster.
   - Saves GO results and generates dot plots for visualization.

5. Output:
   - Saves the clustered gene lists and GO analysis results to files.

Requirement:

To run this script, you need the following R packages:

- `readxl`: For reading Excel files.
- `cluster`: For K-means clustering.
- `clusterProfiler`: For GO enrichment analysis.
- `org.Hs.eg.db`: For gene ID conversion (replace with the appropriate package for your organism).

