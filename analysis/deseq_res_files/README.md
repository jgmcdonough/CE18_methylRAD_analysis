## deseq_res_files

This folder contains the DESeq results (generated from [DESeq_geneFeatureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatureCounts.ipynb) for each of the pairwise comparisons, converted into dataframes and saved as csv files. 

- CC vs. CH = control control vs. control hypoxic
- CC vs. HC = control control vs. hypoxic control
- CC vs. HH = control control vs. hypoxic hypoxic
- CH vs. HC = control hypoxic vs. hypoxic control
- HH vs. CH = hypoxic hypoxic vs. control hypoxic
- HH vs. HC = hypoxic hypoxic vs. hypoxic control
- Hx vs. Cx = phase 1 hypoxic vs. phase 1 control (ignoring effects of phase 2)
- xH vs. xC = phase 2 hypoxic vs. phase 2 control (ignoring effects of phase 1)



In here, you will find:
- all DMGs in each pairwise comparison, regardless of significance
- [sig_DMGs](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/sig_DMGs) - only identified significant DMGs in each pairwise comparison (generated from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb))
- [venn_genes](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/venn_genes) - shared and unique sig. DMGs from venn diagram (genereated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb))
- [GO_terms](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/GO_terms) - GO terms for sig. DMGs (generated from [HC_genes_2.0.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb))
- [go-mwu](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/go-mwu) - output files from GO-MWU analysis using [GO_MWU.R](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/go_mwu/GO_MWU.R) and [mapGO2GOslim.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/mapGO2GOslim.ipynb), contains sig. DMGs with GOslims and GO terms
