# WLS
The Wisconsin Longitudinal Study (WLS, http://www.ssc.wisc.edu/wlsresearch/) is a long-term study of 1957 high school graduates in Wisconsin (N=10317). The survey-based data includes physical and mental health as well as human-human and human-environment interactions from late adolescence (1957) through 2011. These include variables such as social background, aspirations, schooling, military service, labor market experiences, family characteristics and events, social participation, psychological characteristics and retirement.

> Herd, Pamela, Deborah Carr, and Carol Roan. 2014. "Cohort Profile: Wisconsin Longitudinal Study (WLS)." International Journal of Epidemiology 43:34-41 PMCID: PMC3937969

In 2015-6, a microbiota component was added to the WLS with fecal sample collection. The bacterial microbiota was determined by amplicon sequencing of the 16S rRNA gene, variable region 4 (V4). Graduates (g, N=179), their spouses (p, N=63), their siblings (s, N=134), and their sibling's spouses (e, N=32) were successfully sequenced.

This repository contains analyses associated with

> Dill-McFarland KA, Tang Z, Kemis JH, Kerby RL, Chen G, Palloni A, Sorenson T, Rey FE, Herd P. Close social relationships correlate with human gut microbiota composition. *Sci Rep* bioRxiv doi: [10.1101/428938](https://www.biorxiv.org/content/early/2018/09/27/428938).

## Abstract
Social relationships shape human health and mortality via behavioral, psychosocial, and physiological mechanisms, including inflammatory and immune responses. Though not tested in human studies, recent primate studies indicate that the gut microbiome may also be a biological mechanism linking relationships to health. Integrating microbiota data into the 60-year-old Wisconsin Longitudinal Study, we found that socialness with family and friends is associated with differences in the human fecal microbiota. Analysis of spouse (N = 94) and sibling pairs (N = 83) further revealed that spouses have more similar microbiota and more bacterial taxa in common than siblings, with no observed differences between sibling and unrelated pairs. These differences held even after accounting for dietary factors. The differences between unrelated individuals and married couples was driven entirely by couples who reported close relationships; there were no differences in similarity between couples reporting somewhat close relationships and unrelated individuals. Moreover, the microbiota of married individuals, compared to those living alone, has greater diversity and richness, with the greatest diversity among couples reporting close relationships, which is notable given decades of research documenting the health benefits of marriage. These results suggest that human interactions, especially sustained, close marital relationships, influence the gut microbiota.

## Key
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
