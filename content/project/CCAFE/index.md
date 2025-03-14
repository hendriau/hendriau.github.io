---
date: "2024-11-25T00:00:00Z"
external_link: ""
image:
  caption: 
  focal_point: Smart
summary: Estimating Case and Control Allele Frequencies from GWAS Summary Statistics
# website using 
tags:
- Genetics
- Software

authors: 
- HayleyStoneman
- admin

title: Case-Control Allele Frequency Estimation (CCAFE)
links:
- name: Preprint
  url: https://www.biorxiv.org/content/10.1101/2024.10.24.619530v1
- name: Software
  url: https://github.com/wolffha/CCAFE 

---

Methods involving summary statistics in genetics can be quite powerful but can be limited in utility. For instance, many post-hoc analyses of disease studies require case and control allele frequencies (AFs), which are not always published. We present two frameworks to derive case and control AFs from GWAS summary statistics using the odds ratio, case and control sample sizes, and either the total (case and control aggregated) AF or standard error (SE). In simulations and real data, derivations of case and controls AFs using total AF is highly accurate across all settings (e.g., minor AF, condition prevalence). Conversely, derivations using SE underestimate common variant AFs (e.g. minor allele frequency >0.3) in the presence of covariates. We develop an adjustment using gnomAD AFs as a proxy for true AFs, which reduces the bias when using SE. While estimating case and control AFs using the total AF is preferred due to its high accuracy, estimating from the SE can be used more broadly since SE can be derived from p-values and beta estimates, which are commonly provided. The methods provided here expand the utility of publicly available genetic summary statistics and promote the reusability of genomic data. The R package CCAFE, with implementations of both methods, is freely available on Bioconductor and GitHub.
