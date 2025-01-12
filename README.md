Description
This project analyzes RNA A-to-I editing in fly samples, comparing those with Mettl3 modification to control samples. The goal is to evaluate changes in editing levels both overall and in specific genes, determining the statistical significance of these changes.

Input Files
genes_of_interest.tsv: Genomic coordinates for genes to analyze.

Mettl3_1.tsv, Mettl3_2.tsv, Mettl3_3.tsv: Editing data for Mettl3 samples.

Mettl3_ctrl_1.tsv, Mettl3_ctrl_2.tsv, Mettl3_ctrl_3.tsv: Editing data for control samples.

Output
Mean editing change between conditions overall.

Mean editing change for each gene.

P-values indicating statistical significance for overall and individual gene changes.

A bar plot visualizing mean editing changes for each gene.

Usage
Upload Data to Colab: Upload the TSV files to Google Colab.

Run the Code: Execute the code cells in order to perform the analysis.

Interpret Results: Review the output for mean changes and p-values, and visualize the bar plot.

Code Explanation
Step 1: Load necessary libraries.

Step 2: Load input data files.

Step 3: Calculate editing levels as the ratio of G counts to read depth.

Step 4: Combine data for statistical analysis.

Step 5: Compute mean editing changes and p-values for each gene.

Step 6: Perform overall mean editing change analysis.

Step 7: Visualize results with a bar plot.

Dependencies
Ensure you have the necessary libraries installed. These libraries are typically pre-installed in Google Colab.

pandas

numpy

scipy.stats

matplotlib.pyplot
