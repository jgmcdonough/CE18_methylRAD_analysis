## deseq_res_files

This folder contains the DESeq results for each of the pairwise comparisons, converted into dataframes and saved as csv files. 

- CC vs. CH = control control vs. control hypoxic
- CC vs. HC = control control vs. hypoxic control
- CC vs. HH = control control vs. hypoxic hypoxic
- CH vs. HC = control hypoxic vs. hypoxic control
- HH vs. CH = hypoxic hypoxic vs. control hypoxic
- HH vs. HC = hypoxic hypoxic vs. hypoxic control
- Hx vs. Cx = phase 1 hypoxic vs. phase 1 control (ignoring effects of phase 2)
- xH vs. xC = phase 2 hypoxic vs. phase 2 control (ignoring effects of phase 1)

### [DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/DMGs)
DESeq results of differential methylated genes from pairwise comparisons. Contains *all* DMGs, including non-significant genes. CSV files were generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb)


### [DMGs_without_1sample](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/DMGs_without_1sample)
Same as above, but removed a sample we thought might be considered an outlier. CSV files were generated from [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)


### [KEGG_pathways](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/KEGG_pathways)
Enriched KEGG pathways for a pairwise comparison. CSV files were generated from [KEGG_HCgenes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/KEGG_HCgenes.ipynb)


### [sig_DMGs_gene_names](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/sig_DMGs_gene_names)
DESeq results of differential methylated genes from pairwise comparisons. Same as DMGs, but *only* contains significant DMGs and associated gene names from the [NCBI *C. virginica* index database](https://ftp.ncbi.nlm.nih.gov/genomes/all/annotation_releases/6565/100/GCF_002022765.2_C_virginica-3.0/). CSV files were generated from [HC_genes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes.ipynb)


### [venn_genes](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/venn_genes)
CSVs of unique and shared significantly differentially methylated genes from pairwise comparisons that were seen in a Venn diagram. CSV files were generated from [HC_genes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes.ipynb)


_________________________________________________

# [geneFeatures_res](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res)
I had discovered that I had been running my analysis with exons as features and genes as meta-features, so my counts matrix was only counting sequences in exons and binning into genes (I was missing all methylation happening outside of exons (like introns) but inside genes). So, I created a new counts matrix ([geneFeature_counts.txt](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/counts_and_meta/geneFeature_counts.txt)) and re-ran all of my code to generate new files, similar to those above. 

In here, you will find:
- all DMGs in each pairwise comparison, regardless of significance
- [sig_DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/sig_DMGs) - only identified significant DMGs in each pairwise comparison (generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb))
- [venn_genes](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/venn_genes) - shared and unique sig. DMGs from venn diagram (genereated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb))
- [GO_terms](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/GO_terms) - GO terms for sig. DMGs (generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb))
