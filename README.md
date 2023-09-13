# GCase_GWAS

This project assesed genetic variants involved in modifying glucocerebrosidase (GCase) activity in Columbia and PPMI cohorts. The scripts are meant to be run step by step, as they are not optimized for being run with bash and some steps require you to look at the output from previous steps. 

## Outlier removal and normality tests

This is an R script that assesses cohorts for GCase outliers and tests the normality of the data. It also includes investigation into potential interaction effects using interaction plots, ANOVA and linear regressions with interaction terms. File name = "outliers_interaction_plots.R".

## GWAS of GCase

This linux script performs Genome-wide association studies on GCase activity in both independent cohorts, then meta-analyzes the results. Conditional and joint analyses are used to identify secondary associations within significant peaks. We also pull significant SNPs from the Nalls et al. 2019 PD GWAS from the summary statistics of all analyses. File name = "GWAS_COJO.sh"

