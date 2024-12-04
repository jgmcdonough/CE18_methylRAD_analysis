# Figures

## NMDS plots
- [nmds_plot.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot.pdf) - NMDS plot of all genes
- [nmds_plot_sigOnly.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot_sigOnly.pdf) - NMDS plot of only genes that were identified as significantly differentially methylated in at least one pairwise comparison

generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb)


## Volcano plots
volcano plots of *all* six pairwise comparisons - plots differ in how the grids are labbelled (HC vs. Hyp Cont conventions)
- [metaVolcano1.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/metaVolcano1.pdf) - (Hyp Cont convention)
- [metaVolcano2.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/metaVolcano2.pdf) - (HC convention)

Statistically significant differentially methylated genes in each pairwise comparison - data originally generated in [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb), but ggplot generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb)



## DMG_venn
Overlap of differentially methylated genes in pairwise comparisons - data originally generated in [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb), but venn diagram generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb) with ggvenn
