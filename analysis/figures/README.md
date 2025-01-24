# Figures

According to the manuscript:
- **Figure 1**:  Methylation of CpG dinucleotides varies with genomic features and environmental exposure in oysters.
    - **1A**: [new_propOverlap.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/new_propOverlap.pdf), generated from [overlap_genomicFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/overlap_genomicFeatures.ipynb) and visualized with ggplot in [create_proportionPlot.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/create_proportionPlot.ipynb)
    - **1B**: [cpgME_boxplot_faceted.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/cpgMe_boxplot_faceted.pdf), generated from [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb) 
    
- **Figure 2**: The first exposure influences methylation patterns, and differences in the second exposure are observed only after a first exposure to hypoxia.
    - **2A**: [nmds_plot.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot.pdf)
    - **2B**: [nmds_plot_sigOnly.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot_sigOnly.pdf)
    
    both generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb)
    
- **Figure 3**: Timing of hypoxic exposure results in differentially methylated genes
    - **3A**: [metaVolcano2.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/metaVolcano2.pdf) - 
    - **3B**: [DMG_venn.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/DMG_venn.pdf)
    
    DMGs in pairwise comparisons originally generated in [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb), but venn diagram and all volcano plots together generated in [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb) 


# All visualizations and descriptions:

### NMDS plots
- [nmds_plot.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot.pdf) - NMDS plot of all genes
- [nmds_plot_sigOnly.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/nmds_plot_sigOnly.pdf) - NMDS plot of only genes that were identified as significantly differentially methylated in at least one pairwise comparison

generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb)


### Volcano plots
volcano plots of *all* six pairwise comparisons - plots differ in how the grids are labbelled (HC vs. Hyp Cont conventions)
- [metaVolcano1.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/metaVolcano1.pdf) - (Hyp Cont convention)
- [metaVolcano2.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/metaVolcano2.pdf) - (HC convention)

Statistically significant differentially methylated genes in each pairwise comparison - data originally generated in [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb), but ggplot generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb)



### Venn diagrams
- [DMG_venn.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/DMG_venn.pdf) - Overlap of DMGs in pairwise comparisons - data originally generated in [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb), but venn diagram generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb) with ggvenn
- [exonME_venn.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/exonMe_venn.pdf) - overlap of methylated exons between treatments, generated in [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb)
- [cpgMe_venn.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/cpgMe_venn.pdf) - overlap of methylated CpG dinucleotides between treatments, generated in [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb)


### Proportion Overlap
- [propOverlap.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/propOverlap.pdf) - for each treatment, the proportion of methylated CpGs that overlap with genomic features - data generated from [overlap_genomicFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/overlap_genomicFeatures.ipynb) and visualized with ggplot in [create_proportionPlot.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/create_proportionPlot.ipynb)

### Methylation Level Boxplots
- [cpgME_boxplot_faceted.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/cpgMe_boxplot_faceted.pdf) - CpG dinucleotide methylation (>5 methylRAD sequences) level (methylated CpG/total CpG * 100) - data generated from [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb) 
