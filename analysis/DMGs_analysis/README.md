# DMGs_analysis
Scripts for identifying differential methylation 

### 1. [featureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/featureCounts.ipynb)
generates counts matrix of features (i.e., exons) and meta-features (i.e., genes)

### 2. [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)
Identifies significantly differentially methylated genes in pairwise comparisons, as well as NMDS plots

### 3. [HC_genes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes.ipynb)
Volcano plots of DESeq results (ggplot) and other downstream analysis (Venn diagram, GO terms)


#### shorthand:
Throughout these scripts, I use shorthand for the treatments:
- H = hypoxic
- C = control
- Phase1Phase2 

so for example, HC = hypoxic control = phase 1 was hypoxic, phase 2 was control