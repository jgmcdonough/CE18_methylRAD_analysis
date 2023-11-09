# CE_MethylRAD_analysis_2018
carryover effects DNA methylation analysis for eastern oysters (Crassostrea virginica) using MethylRAD - samples and sequences from Sarah in 2018

Reference Genome used: 
NCBI RefSeq assembly: GCF_002022765.2 https://www.ncbi.nlm.nih.gov/genome/annotation_euk/Crassostrea_virginica/100/

GCA_002022765.4_C_virginica-3.0_genomic.fna https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_002022765.2/

## CE_methyl_QC.ipynb
This file includes all of the code used to quality check and clean sequences to prep for analysis. 
1. fastqc and multiqc samples - check raw sequence quality
2. trim - used trim-galore with auto-detect adapters and filtered for smaller bp sequences
3. fastqc and multiqc on the trimmed and filtered sequences to check quality again
4. using GenBank reference genome, index and align with bowtie2 - check alignment rates
5. converting SAM files to BAM files, then sorting the BAM files
6. using picard to mark duplicates
7. indexing sorted BAM files
8. using htseq-counts to record the number of counts for each feature

## pipeline_counts.ipynb
Getting the read counts for each step of the pipeline: number of raw reads and trimmed reads, number of reads that aligned concordantly to the NCBI RefSeq, number of marked duplicates, and the number of reads that were aligned to features with htseq-counts

## picard.jar
This is the picard package in order to use picard tools to mark duplicates




