# DMGs_analysis
Scripts for identifying differential methylation 

Anything related to gene ontology can be found in the [GeneOntology](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/GeneOntology) directory

### 1. [featureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/featureCounts.ipynb)
Generates counts matrix of sequences occurring withing a gene region (as identified in annotation file)
- [geneFeature_counts.txt](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/counts_and_meta/geneFeature_counts.txt)

### 2A. [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)
Identifies significantly differentially methylated genes in pairwise comparisons, as well as NMDS plots
- [DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res) - directory containing DESeq results for *all* genes in each pairwise comparison (regardless if significant or not), as well as additional sub-directories
- [sig_DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/sig_DMGs) - folder containing all significantly DMGs for each pairwise comparison, with the associated gene name according to the GCF annotation file from NCBI

### 2B. [volcano_DESeq.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/volcano_DESeq.ipynb)
takes the results from [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb), combine files into one df, and create grid of DESeq volcano plots using ggplots

### 3. [DMGs.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DMGs.ipynb)
Downstream analysis from DESeq results (idnividual volcano plots, venn diagrams of shared and unique DMGs, GO terms of DMGs)
- [GO_terms](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/GeneOntology) - folder containing GO terms for each pairwise comparison with HC
- [venn_genes](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/venn_genes) - folder containing shared and unique DMGs in pairwise comparisons from the venn diagram 


#### shorthand:
Throughout these scripts, I use shorthand for the treatments:
- H = hypoxic
- C = control
- Phase1Phase2 

so for example, HC = hypoxic control = phase 1 was hypoxic, phase 2 was control