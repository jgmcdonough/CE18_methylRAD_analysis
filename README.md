# Carryover effects of early life hypoxia influences DNA methylation in *Crassostrea virginica*

Raw sequence data is available at the NCBI Sequence Read Archive under BioProject accession number PRJNA1327452.

## Background
Environmentally-induced epigenetics, like DNA methylation, can help organisms adapt and respond to the increasingly variable environments produced by climate change. Less well-understood is how methylation may encode memory of past environments and influence the response to current environments (i.e., carryover effects). In a fully factorial experiment, we exposed juvenile eastern oysters (Crassostrea virginica) to two phases of water treatments with manipulated dissolved oxygen (control or hypoxia, <2 mg/L) to simulate climate change predictions and processed whole-body tissues for MethylRAD-sequencing. 


NCBI RefSeq assembly: [GCF_002022765.2](https://www.ncbi.nlm.nih.gov/genome/annotation_euk/Crassostrea_virginica/100/)


## Results

### [Quality Check](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/quality_check)
contains scripts and files used to quality check sequences in prep for analysis

### [Pipeline Counts](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/pipeline_counts)
contains scripts and files of sequences counts per sample for each step in quality pipeline

### [Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis)
contains scripts and generated data files/figures from the various analyses
- **[Differential Methylation Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/DMGs_analysis)** - identified significantly differentially methylated genes between treatments
- **[DESeq2 results](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files)** - CSVs of DESeq results for each pairwise comparison. Incldues both non-significant and significant differentially methylated genes. 
- **[Counts matrix & meta data](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/counts_and_meta)** - Inputs for DESeq analysis. Counts matrix of features and meta-features (featureCounts) and meta data about the samples.








