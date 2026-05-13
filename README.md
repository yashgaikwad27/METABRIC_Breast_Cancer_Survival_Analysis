# METABRIC Breast Cancer Survival Analysis

## Overview
Survival analysis of 1,466 breast cancer patients from the METABRIC dataset in R, examining mortality risk across tumor stages and key clinical predictors including ER, PR, and HER2 status.

## What I Did
- Cleaned and prepared clinical data, handling missing values and recoding variables for survival analysis
- Estimated overall and stage-stratified survival curves using Kaplan-Meier methods, confirming significant survival differences across tumor stages (p < 0.0001)
- Ran a multivariable Cox proportional hazards model with age, tumor stage, size, grade, ER, PR, and HER2 status
- Identified proportional hazards violations across multiple covariates using Schoenfeld residual diagnostics
- Built a revised model stratifying on tumor stage and modeling age as a time-dependent covariate to appropriately address PH violations

## Tools & Methods
R, R Markdown, tidyverse, survival, survminer, Kaplan-Meier, Cox Proportional Hazards, Schoenfeld Residuals, Time-Dependent Covariates

## Files
- `METABRIC_Survival.Rmd` - Full analysis code
- `METABRIC_Survival.pdf` - Knitted output with results and visualizations
