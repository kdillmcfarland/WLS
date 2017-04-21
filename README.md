# WLS
The Wisconsin Longitudinal Study (WLS, http://www.ssc.wisc.edu/wlsresearch/) is a long-term study of 1957 high school graduates in Wisconsin (N=10317). The survey-based data includes physical and mental health as well as human-human and human-environment interactions from late adolescence (1957) through 2011. These include variables such as social background, aspirations, schooling, military service, labor market experiences, family characteristics and events, social participation, psychological characteristics and retirement.

> Herd, Pamela, Deborah Carr, and Carol Roan. 2014. "Cohort Profile: Wisconsin Longitudinal Study (WLS)." International Journal of Epidemiology 43:34-41 PMCID: PMC3937969

In 2015-6, a microbiota component was added to the WLS with fecal sample collection. The bacterial microbiota was determined by amplicon sequencing of the 16S rRNA gene, variable region 4 (V4). Graduates (g, N=179), their spouses (p, N=63), their siblings (s, N=134), and their sibling's spouses (e, N=32) were successfully sequenced.

This repository contains files associated with microbiota analysis of WLS. 


R markdown

  * WLS_mothur - mothur code for processing fastq files into an OTU table
  * WLS_data_manipulation - manipulation of the WLS and microbiota data sets to be used in analysis
  * WLS_analysis - statistical analyses of WLS and microbiota data sets

R scripts
  * Pairwise_adonis.R - Pairwise PERMANOVA (adonis) function to test within categorical variables with more than 2 levels
  * R_krusk.R	- Function to calculate Kruskal-Wallis for OTUs and variables identified in SIMPER analysis
  * multiplot.R - Function to place 2 or more ggplot2 graphs in one figure

python scripts
  * clean_repFasta_FAST.py - Renames sequences in representative sequence fasta file to OTU numbers (i.e. Otu0001, Otu0002, etc.)
