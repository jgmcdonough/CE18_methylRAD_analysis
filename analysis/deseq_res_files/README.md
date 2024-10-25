## deseq_res_files

This folder contains the DESeq results for each of the pairwise comparisons, converted into dataframes and saved as csv files. These contains *all* of the genes, including non-significant DMGs. 

- CC vs. CH = control control vs. control hypoxic
- CC vs. HC = control control vs. hypoxic control
- CC vs. HH = control control vs. hypoxic hypoxic
- CH vs. HC = control hypoxic vs. hypoxic control
- HH vs. CH = hypoxic hypoxic vs. control hypoxic
- HH vs. HC = hypoxic hypoxic vs. hypoxic control
- Hx vs. Cx = phase 1 hypoxic vs. phase 1 control (ignoring effects of phase 2)
- xH vs. xC = phase 2 hypoxic vs. phase 2 control (ignoring effects of phase 1)


any csv with 'WO' in the front stands for **without**, as in, removal of 'outlier' sample (WBO-BBR-W03) that was identified in the NMDS plots. I did the same analysis without it to see if there were any major changes in the analysis by removing it. 


csv files with KEGG at the beginning are enriched pathways identified from the differentially methylated genes in that pairwise comparison.