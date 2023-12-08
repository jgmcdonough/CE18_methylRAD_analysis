# CE_MethylRAD_analysis_2018
carryover effects DNA methylation analysis for eastern oysters (Crassostrea virginica) using MethylRAD - samples and sequences from Sarah Gignoux-Wolfsohn in 2018

Reference Genome used: 
NCBI RefSeq assembly: GCF_002022765.2 https://www.ncbi.nlm.nih.gov/genome/annotation_euk/Crassostrea_virginica/100/
GTF file: https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_002022765.2/

## CE_methyl_QC
This folder includes all files used/needded to quality check and process reads for downstream analysis.

#### CE_methyl_QC.ipynb
This file includes all of the code used to quality check and clean sequences to prep for analysis, including alignment. 

## CE_methyl_analysis
This folder includes all files used/needed for analysis of methylRAD sequences.

#### CE_methyl_analysis.ipynb
Jupyter notebook for data analysis using DESeq2.

#### counts_and_meta
Folder containing all files needed as input for analysis. These include:
- **counts_exon.txt:** counts matrix generated with htseq-counts with type=exon.
- **counts_gene.txt:** counts matrix generated with htseq-counts with type=gene.
- **CV_CE18_meta.csv:** table containing the meta data for the CV samples.

#### figures
Folder containing all of the figures and plots produced from analysis with DESeq2. 

#### significant_genes
Folder containing csv files generated from DESeq analysis for identified significant genes for that treatment.
- **sig_hw_genes.csv:** data table with info for sig. genes for all hypoxic warm treatment 2 samples and comparing treatment 1 methylation.
- **sig_T1_temp.csv:** data table with info for sig. genes for warm vs. ambient samples for treatment 1.
- **sig_TC1_normoxic.warm_vs_hypoxic.ambient.csv:** data table with info for sig. genes for normoxic warrm vs. hypoxic ambient for treatment 1.

## pipeline_counts
This folder contains all files used/needed for pipeline read counts for each sample.

#### pipeline_counts.ipynb
Getting the read counts for each step of the pipeline: number of raw reads and trimmed reads, number of reads that aligned concordantly to the NCBI RefSeq, number of marked duplicates, and the number of reads that were aligned to features with htseq-counts

#### CV_CE18_pipeline_counts.csv
Table containing the amount of reads after each step in the quality-check pipeline. The marked_dup column is the number of marked optical duplicates of the read pairs. 








