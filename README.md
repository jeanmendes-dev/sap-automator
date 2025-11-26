# 📊 r-sap-automator  
*Automated Statistical Analysis Plan (SAP) Template in R — ICH E9 Compliant*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![R](https://img.shields.io/badge/R-≥4.0-3572A5?logo=r)](https://www.r-project.org)
[![officedown](https://img.shields.io/badge/officedown-✓-blue)](https://davidgohel.github.io/officedown/)
[![flextable](https://img.shields.io/badge/flextable-✓-purple)](https://davidgohel.github.io/flextable/)

> A fully reproducible, RMarkdown-based Statistical Analysis Plan (SAP) template aligned with **ICH E9** guidelines — generating professional Word documents with dynamic tables, figures, and regulatory-grade structure.

---

## 🎯 Why This Matters

In clinical research, **SAPs must be pre-specified, version-controlled, and audit-ready**. Manual Word documents are error-prone and non-reproducible.

This template solves that by:

✅ Automating SAP generation with R  
✅ Ensuring ICH E9 compliance (full section coverage)  
✅ Enabling parameterization (study name, endpoints, sample size, etc.)  
✅ Producing publication-ready `.docx` output with TOC, tables, and figures  
✅ Supporting traceability, version control, and audit trails  

Ideal for biostatisticians, statistical programmers, and regulatory teams.

---

## 📸 Output Preview

| Section | Screenshot |
|--------|------------|
| **Table of Contents** | ![TOC](sap_template_img1.png) |
| **Analysis Populations Table** | ![Populations](sap_template_img2.png) |
| **Demographic Table** | ![Demo](sap_template_img3.png) |
| **Boxplot Figure (Baseline HbA1c)** | ![Figure](sap_template_img4.png) |
| **Adverse Events Table** | ![AE](sap_template_img5.png) |

---

## 🚀 Quick Start

### Prerequisites
- R ≥ 4.0  
- RStudio (recommended)  
- Packages: `rmarkdown`, `officedown`, `flextable`, `officer`, `dplyr`, `ggplot2`

```r
install.packages(c(
  "rmarkdown", "officedown", "flextable", "officer",
  "dplyr", "ggplot2", "knitr"
))
```
### Generate Your SAP
 - Open `sap_template.Rmd` in RStudio
 - Edit `study_params` in the setup chunk (lines 10–20)
   
```r
study_params <- list(
  study_name = "Your Study Name",
  sponsor = "Your Sponsor",
  protocol_number = "PROT-123",
  primary_endpoint = "Change in HbA1c at Week 24",
  sample_size = 350,
  ...
)
```
 - Click Knit → Generates sap_template.docx in your working directory.
