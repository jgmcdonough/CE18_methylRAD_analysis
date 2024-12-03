# DMGs_analysis
Scripts for identifying differential methylation 

### 1. [featureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/featureCounts.ipynb)
Generates counts matrix of sequences occurring withing a gene region (as identified in annotation file)
- [geneFeature_counts.txt](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/counts_and_meta/geneFeature_counts.txt)

### 2. [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)
Identifies significantly differentially methylated genes in pairwise comparisons, as well as NMDS plots
- [DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res) - directory containing DESeq results for *all* genes in each pairwise comparison (regardless if significant or not), as well as additional sub-directories
- [sig_DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/sig_DMGs) - folder containing all significantly DMGs for each pairwise comparison, with the associated gene name according to the GCF annotation file from NCBI

### 3A. [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb)
Downstream analysis from DESeq results (volcano plots, venn diagrams of shared and unique DMGs, GO terms of DMGs)
- [GO_terms](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/GO_terms) - folder containing GO terms for each pairwise comparison with HC
- [venn_genes](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/venn_genes) - folder containing shared and unique DMGs in pairwise comparisons from the venn diagram 

### 3B. [KEGG_HCgenes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/KEGG_HCgenes_2.0.ipynb)
Further downstream analysis from DESeq - KEGG analysis

### 3C. [genes_pathway_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/genes_pathway_analysis.ipynb)
Are the significant DMGs identified in DESeq the core enrichment genes in identified enriched pathways from KEGG?

#### shorthand:
Throughout these scripts, I use shorthand for the treatments:
- H = hypoxic
- C = control
- Phase1Phase2 

so for example, HC = hypoxic control = phase 1 was hypoxic, phase 2 was control