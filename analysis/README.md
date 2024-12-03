# CE18 MethylRAD Analysis
This directory contains all scripts, files, and figures generated during analysis of the methylRAD sequences.

### [DMGs_analysis](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/DMGs_analysis)
Differential methylation analysis scripts
- 01. [featureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/featureCounts.ipynb) - generate counts matrix of gene regions ([geneFeature_counts.txt](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/counts_and_meta/geneFeature_counts.txt))
- 02. [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb) - run DESeq2 on counts matrix, create csv files of differentially methylated genes for each pairwise comparison - output in the [geneFeatures_res](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res) folder
- 03. [HC_genes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/HC_genes_2.0.ipynb) - downstream analysis of DESeq2; input is [DESeq files](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res) and creates volcano plots, [venn diagram](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/venn_genes), [GO terms](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files/geneFeatures_res/GO_terms)
- 04. [KEGG_HCgenes.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/KEGG_HCgenes_2.0.ipynb) - KEGG pathway enrichment analysis for each pairwise comparison with HC oysters


### [counts_and_meta](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/counts_and_meta)
Counts matrices generated from [featureCounts.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/featureCounts.ipynb), meta data of oysters (treatment information, phenotype data)


### [deseq_res_files](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/deseq_res_files)
Results of pariwise comparisons from [DESeq_geneFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/DMGs_analysis/DESeq_geneFeatures.ipynb)


### [genomic_feature_tracks](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/genomic_feature_tracks)
Scripts to generate and analyze genomic features in the oyster genome, as well as the genomic feature tracks (BED and GFF3 files) themselves. Above, I counted sequences within a defined gene region and asked if there were differentially methylated genes between treatments. Here, I identified methylated CpG dinucleotides (5x coverage was considered methylated) and analzyed the overlap of these methylated CpG dinucleotides with other genomic features (i.e., exons, introns, CDS, intergenic regions, non-coding regions, exon UTRs, transposable elements, mRNA) for each treatment combination. I was able to calculate methlyation level of various genomic features (number of methylated feature/total number of feature) as well.

Genomic feature track files were generated with [generate_genomic_feature_tracks.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/generate_genomic_feature_tracks.ipynb) and further analyzed with [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb)

### [phenotype_data.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/phenotype_data.ipynb)
Phenotype data (tissue and shell growth) for the oysters analyzed.

