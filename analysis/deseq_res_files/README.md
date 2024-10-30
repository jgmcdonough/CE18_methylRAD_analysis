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
DESeq results of differential methylated genes from pairwise comparisons. Contains *all* DMGs, including non-significant genes. CSV files were generated from [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)


### [DMGs_without_1sample](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/DMGs_without_1sample)
Same as above, but removed a sample we thought might be considered an outlier. CSV files were generated from [DESeq_analysis.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_analysis.ipynb)


### [KEGG_pathways](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/KEGG_pathways)
Enriched KEGG pathways for a pairwise comparison. CSV files were generated from [KEGG_HCgenes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/KEGG_HCgenes.ipynb)


### [sig_DMGs_gene_names](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/sig_DMGs_gene_names)
DESeq results of differential methylated genes from pairwise comparisons. Same as DMGs, but *only* contains significant DMGs and associated gene names from the [NCBI C. virginica index database](https://ftp.ncbi.nlm.nih.gov/genomes/all/annotation_releases/6565/100/GCF_002022765.2_C_virginica-3.0/). CSV files were generated from [HC_genes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes.ipynb)
