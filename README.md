# RNA A-to-I Editing Statistical Analysis

**Notice**: This code is shared for educational and demonstration purposes only. No permission is granted to use, modify, reproduce, or distribute this code or any part of it without explicit prior written consent from the author. Please refer to the License section for further details.

## Table of Contents

- [Description](#description)
- [Input Files](#input-files)
- [Output](#output)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Dependencies](#dependencies)
- [License](#license)

## Description

This project analyzes RNA A-to-I editing in fly samples, comparing those with Mettl3 modification to control samples. The goal is to evaluate changes in editing levels both overall and in specific genes, determining the statistical significance of these changes.

## Input Files

- `genes_of_interest.tsv`: Genomic coordinates for genes to analyze.
- `Mettl3_1.tsv`, `Mettl3_2.tsv`, `Mettl3_3.tsv`: Editing data for Mettl3 samples.
- `Mettl3_ctrl_1.tsv`, `Mettl3_ctrl_2.tsv`, `Mettl3_ctrl_3.tsv`: Editing data for control samples.

## Output

- Mean editing change between conditions overall.
- Mean editing change for each gene.
- P-values indicating statistical significance for overall and individual gene changes.
- A bar plot visualizing mean editing changes for each gene.

## Usage

1. **Upload Data to Colab**: Upload the TSV files to Google Colab.
2. **Run the Code**: Execute the code cells in order to perform the analysis.
3. **Interpret Results**: Review the output for mean changes and p-values, and visualize the bar plot.

## Code Explanation

1. **Step 1**: Load necessary libraries.
2. **Step 2**: Load input data files.
3. **Step 3**: Calculate editing levels as the ratio of G counts to read depth.
4. **Step 4**: Combine data for statistical analysis.
5. **Step 5**: Compute mean editing changes and p-values for each gene.
6. **Step 6**: Perform overall mean editing change analysis.
7. **Step 7**: Visualize results with a bar plot.

## Dependencies

Ensure you have the necessary libraries installed. These libraries are typically pre-installed in Google Colab.

- `pandas`
- `numpy`
- `scipy.stats`
- `matplotlib.pyplot`

Alternatively, if running locally, install them using:

```bash
pip install pandas numpy scipy matplotlib
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

If you want more control, you can write a custom license that explicitly states your terms. For example:

**Custom License Template:**
```plaintext
Copyright (c) [2025] [Rami BABAS]. All rights reserved.

This code is part of a research project and is provided for academic and educational purposes. No permission is granted to use, modify, reproduce, or distribute this code or any derivatives without explicit prior written consent from the author.
```
