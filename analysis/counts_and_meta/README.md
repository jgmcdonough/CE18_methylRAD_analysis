# Counts and meta data
This folder contains all of the input files for downstream analysis - mainly counts matrix and meta data.


# Meta data

### CV_CE18_meta.csv
Meta data for all of the samples - phase 1 temperature and DO treatment, phase 2 temperature and DO treatment, code names, original sample names, etc.

### CV_CE_phenotype_meta.csv
Meta data for all of the samples, as well as growth data for the tissue and shell.


# Counts matrices

### counts_formatted.csv
Counts matrix of meta-features that is used for DESeq analysis.

### counts_meta.csv
Like counts_formatted.csv but contains information from the GFF file (chromosome, start and end position, gene_id info, etc.