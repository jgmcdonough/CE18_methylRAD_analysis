# Genomic feature tracks
This directory has scripts that generated each genomic feature track, as well as the BED and GFF3 files for each feature track. Most of these feature tracks were generated following the pipeline by Dr. Yaamini R. Venkataraman ([paper-gonad-meth repo](https://github.com/epigeneticstoocean/paper-gonad-meth/tree/master))


## Scripts

#### [generate_genomic_feature_tracks.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/generate_genomic_feature_tracks.ipynb) 
This script utilizes the [BEDtools suite](https://bedtools.readthedocs.io/en/latest/content/bedtools-suite.html) in command line to generate various feature tracks from the [NCBI *C. virginica* GCF annotation file](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_002022765.2/)

#### [methylation_level_of_features.ipynb](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/methylation_level_of_features.ipynb)
This script uses the genomic feature files generated from the script above to analyze where methylation is happening in oysters by determining overlap with genomic features, as well as percent methylation of certain features. 


## Files
All genomic feature tracks were generated from the above script

#### [generating_promoter_track](https://github.com/jgmcdonough/CE18_methylRAD_analysis/tree/master/analysis/genomic_feature_tracks/generating_promoter_track)
This directory contains all of the intermediary files generated to get the final [mRNA_promoter_track.bed](https://github.com/jgmcdonough/CE18_methylRAD_analysis/blob/master/analysis/genomic_feature_tracks/mRNA_promoter_track.bed) file.