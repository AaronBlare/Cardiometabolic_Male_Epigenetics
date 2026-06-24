
# Epigenetic Signatures of Cardiometabolic Risk in Men: Accelerated Aging and Differential Methylation Replicated Across Cohorts

Repository with source code for paper "Epigenetic Signatures of Cardiometabolic Risk in Men: Accelerated Aging and Differential Methylation Replicated Across Cohorts" by 
[A. Kalyakulina](https://orcid.org/0000-0001-9277-502X),
[I. Yusipov](http://orcid.org/0000-0002-0540-9281),
F. Botasheva,
[N. Bujlova](https://orcid.org/0000-0002-0604-6603),
[E. Zagaynova](https://orcid.org/0000-0003-2097-0525),
[C. Franceschi](http://orcid.org/0000-0001-9841-6386),
[M. Ivanchenko](http://orcid.org/0000-0002-1903-7423). 

## Description 

This repository contains source code for plotting figures and performing epigenetic profiles analysis.

## Abstract
Background: Men exhibit greater susceptibility to cardiovascular diseases and metabolic disorders, with an earlier onset and more aggressive progression, which may be driven by epigenetic modifications, particularly DNA methylation. Our goal was to comprehensively characterize the epigenetic landscape of a broad cardiometabolic burden in a cohort consisting exclusively of men.

Results: We generated novel DNA methylation profiles from whole blood of men with cardiometabolic disturbances (diagnosed with hypertension, ischemic heart disease, obesity, dyslipidemia) and age-matched healthy controls. Cases demonstrated significant epigenetic age acceleration, most pronounced for second-generation clocks (GrimAge, GrimAge2) and pace of aging measures (DunedinPACE), accompanied by shortened epigenetic telomere length (DNAmTL). Markedly, none of 19 evaluated first-generation epigenetic clocks exhibited sensitivity to the studied diseases. Epigenome-wide association analysis identified numerous differentially methylated positions (DMPs), predominantly hypomethylated in cases compared to controls. Gene set enrichment analysis of genes annotated to these DMPs revealed nine distinct biological pathway clusters collectively reflecting the multifactorial processes associated with cardiometabolic burden, including chronic inflammation, GPCR signaling dysregulation, metabolic disturbances, mitochondrial dysfunction, vascular remodeling, and renal electrolyte regulation. Crucially, key findings, including GrimAge acceleration, DunedinPACE elevation, DNAmTL shortening, and enrichment of inflammatory and GPCR pathways, were replicated in an independent cohort of men with atherosclerosis.

Conclusions: Men with cardiometabolic disturbances exhibit accelerated epigenetic aging and distinct DNA methylation signatures associated with cardiometabolic burden. A comprehensive analysis of an extensive battery of epigenetic clock models revealed that only the second-generation (GrimAge) and third-generation (DunedinPACE) models demonstrated a pronounced sensitivity to the evaluated uncomplicated diseases. In contrast, the first-generation models, trained to predict chronological age, failed to detect significant differences between the groups, suggesting their limited applicability in the context of these pathologies. The concordance of results across original and independent replication cohorts underscores the fundamental nature of these epigenetic alterations. Our findings suggest candidate biomarkers measurable in minimally invasive blood samples that may assist in early risk stratification and monitor disease progression in men, warranting further prospective evaluation for clinical translation.

## Project Structure

```
├── Original                       <- Scripts for the original dataset
│   ├── data                        <- Data and generated results
│   ├── 01_preprocess.r             <- Data preprocessing
│   ├── 02_ewas_gsea.r              <- EWAS and GSEA analysis
│   └── 03_statistics.ipynb         <- Statistical analysis for epigenetic ages, metrics, EpiScores, blood cells estimates
├── GSE220622                      <- Scripts for the external dataset GSE220622
│   ├── data                        <- Data and generated results
│   ├── 01_preprocess.r             <- Data preprocessing
│   ├── 02_ewas_gsea.r              <- EWAS and GSEA analysis
│   └── 03_statistics.ipynb         <- Statistical analysis for epigenetic ages, metrics, EpiScores, blood cells estimates
├── .gitignore                     <- List of files ignored by git
├── .project-root                  <- File for inferring the position of project root directory
├── requirements.txt               <- File for installing python dependencies
└── README.md                      <- This file
```

## Install dependencies

```bash
# clone project
git clone https://github.com/AaronBlare/Cardiometabolic_Male_Epigenetics
cd Cardiometabolic_Male_Epigenetics

# [OPTIONAL] create conda environment
conda create -n env_name python=3.12
conda activate env_name

# install requirements
pip install -r requirements.txt
```
