# Human Airway Transcriptomics: Differential Gene Expression Analysis via DESeq2

This repository features an end-to-end biostatistical transcriptomic analysis pipeline utilizing the `DESeq2` framework in R to isolate differentially expressed genes (DEGs) in human airway smooth muscle cells following dexamethasone treatment.

## Analysis Workflow
* **Dataset:** Public `airway` high-throughput RNA-Seq count matrix (4 treated vs 4 untreated samples).
* **Normalization & Statistics:** Negative binomial generalized linear models via Bioconductor's `DESeq2`.
* **Threshold Metrics:** Adjusted p-value cutoff $< 10^{-6}$ and $|\log_2\text{FoldChange}| > 1.5$.

## Technical Stack
* **Language:** R
* **Ecosystem:** Bioconductor
* **Core Libraries:** `DESeq2`, `EnhancedVolcano`, `airway`

## Key Finding
The workflow successfully handles downstream expression matrices, controls for high-dimensional false discovery rates, and generates a publication-ready Volcano Plot mapping statistically significant transcriptional adjustments.
