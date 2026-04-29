
# CE_MethylRAD_analysis

[![DOI](zenodo.org)](https://doi.org/10.5281/zenodo.17902788)

<img width="2880" height="1620" alt="McDonough2026_graphAbstract" src="https://github.com/user-attachments/assets/8e24f49b-bf69-406d-b1fc-436298e88697" />


This repository includes data and analysis scripts to accompany:

## Manuscript Info
**Title**: Prior exposure to hypoxia alters DNA methylation patterns in the eastern oyster

**DOI**: https://doi.org/10.1186/s12864-026-12808-6

**Authors**: Julia G. McDonough<sup>1</sup>, Thomas J. Miller<sup>2</sup>, Teresa W. Lee<sup>1</sup>, Sarah C. Donelan<sup>3</sup>, Sarah A. Gignoux-Wolfsohn<sup>1</sup>

<sup>1</sup>University of Massachusetts Lowell

<sup>2</sup>University of Maryland Center for Environmental Science

<sup>3</sup>University of Massachusetts Dartmouth


**Abstract**: Environmentally induced epigenetic changes (e.g., DNA methylation) can alter genetic activity to help organisms adapt and respond to variable environments. While many studies have investigated DNA methylation as a response to a stressor at a single timepoint, less well-understood is how methylation may encode memory of past environments and influence the response to current environments (i.e., carryover effects). Oysters are an excellent natural system to study carryover effects due to their sessile nature, which may expose them to increased environmental variability. To better understand how methylation changes in response to a previous exposure of environmental stress, we conducted a fully factorial experiment exposing juvenile oysters to either control or hypoxic conditions at two timepoints separated by 60 days. After the second exposure, whole body tissue samples were collected and processed for methylRAD sequencing. Regardless of treatment, methylation was mostly found in exons. We found both the first and second exposure treatments contributed significantly to the observed variation in gene body methylation. Interestingly, oysters that were first exposed to hypoxia and later exposed to control conditions had methylation patterns that differed the most from any other condition. We found that differentially methylated genes identified in pairwise comparisons were mainly involved in the oxidative stress response, metabolism, and transcription. Together, these findings suggest that early life environments have a lasting impact on the epigenome and that the timing of stress elicits unique response strategies, which highlights potential targets of resilience for oysters. 


## Sequence Info
Raw sequence data is available at the NCBI Sequence Read Archive under BioProject accession number PRJNA1327452.


NCBI RefSeq assembly: [GCF_002022765.2](https://www.ncbi.nlm.nih.gov/genome/annotation_euk/Crassostrea_virginica/100/)


## Directory Info

### [Quality Check](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/quality_check)
contains scripts and files used to quality check sequences in prep for analysis

### [Processing](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/processing)
contains scripts and files of sequences counts per sample for each step in quality pipeline

### [Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis)
contains scripts and generated data files/figures from the various analyses
- **[Differential Methylation Analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/DMGs_analysis)** - identified significantly differentially methylated genes between treatments
- **[DESeq2 results](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files)** - CSVs of DESeq results for each pairwise comparison. Incldues both non-significant and significant differentially methylated genes. 
- **[Counts matrix & meta data](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/counts_and_meta)** - Inputs for DESeq analysis. Counts matrix of features and meta-features (featureCounts) and meta data about the samples.








