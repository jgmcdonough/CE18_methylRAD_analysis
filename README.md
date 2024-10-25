# CE_MethylRAD_analysis_2018
carryover effects DNA methylation analysis for eastern oysters (Crassostrea virginica) using MethylRAD - samples and sequences from Dr. Sarah Gignoux-Wolfsohn in 2018

**Reference Genome files used:**

NCBI RefSeq assembly: GCF_002022765.2 https://www.ncbi.nlm.nih.gov/genome/annotation_euk/Crassostrea_virginica/100/

GTF file: https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_002022765.2/


## [Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis)
contains scripts and generated data files/figures from the various analyses
- **[Differential Methylation Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/DMGs_analysis)** - identified significantly differentially methylated genes between treatments
- **[DESeq2 results](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files)** - CSVs of DESeq results for each pairwise comparison. Incldues both non-significant and significant differentially methylated genes. 
- **[Counts matrix & meta data](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/counts_and_meta)** - Inputs for DESeq analysis. Counts matrix of features and meta-features (featureCounts) and meta data about the samples.

## [Pipeline Counts](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/pipeline_counts)
contains scripts and files of sequences counts per sample for each step in quality pipeline

## [Quality Check](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/quality_check)
contains scripts and files used to quality check sequences in prep for analysis








