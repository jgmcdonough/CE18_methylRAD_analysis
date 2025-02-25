# Genomic feature tracks
This directory has scripts that generated each genomic feature track, as well as the BED and GFF3 files for each feature track. Most of these feature tracks were generated following the pipeline by Dr. Yaamini R. Venkataraman ([paper-gonad-meth repo](https://github.com/epigeneticstoocean/paper-gonad-meth/tree/master))


## Scripts

#### [generate_genomic_feature_tracks.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/generate_genomic_feature_tracks.ipynb) 
This script utilizes the [BEDtools suite](https://bedtools.readthedocs.io/en/latest/content/bedtools-suite.html) in command line to generate various feature tracks from the [NCBI *C. virginica* GCF annotation file](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_002022765.2/)

#### [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb)
This script uses `bedtools multicov` with the CpG motif file to map methylRAD sequences to CpG dinucleotides for each oyster. Generates [cpgME_boxplot_faceted.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/cpgMe_boxplot_faceted.pdf)


## Files
All genomic feature tracks were generated from the above script

#### [generating_promoter_track](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/genomic_feature_tracks/generating_promoter_track)
This directory contains all of the intermediary files generated to get the final [mRNA_promoter_track.bed](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/mRNA_promoter_track.bed) file.

#### [proportion_overlap](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/genomic_feature_tracks/proportion_overlap)
This directory contains all files and scripts related to determining overlap of methylated CpGs with genomic features (using [overlap_genomicFeatures.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/proportion_overlap/overlap_genomicFeatures.ipynb)), as well as generating [propOverlap_faceted.pdf](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/figures/propOverlap_faceted.pdf) (using [create_proportionPlot.ipynb]((https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/proportion_overlap/create_proportionPlot.ipynb)) - code is in different languages, hence two separate scripts