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
| **Table of Contents + General Info** | ![TOC](https://via.placeholder.com/600x200/e0e0e0/000000?text=TOC+%26+Study+Info) |
| **Analysis Populations Table** | ![Populations](https://via.placeholder.com/600x150/f5f5f5/333333?text=Table+1:+Analysis+Populations) |
| **Demographics + Safety Table** | ![Demo](https://via.placeholder.com/600x180/f8f9fa/212529?text=Table+2:+Demographics+%26+AEs) |
| **Boxplot Figure (Baseline HbA1c)** | ![Figure](https://via.placeholder.com/600x300/ffffff/000000?text=Figure+1:+Baseline+HbA1c+Distribution) |

> 🔁 Replace placeholders with actual screenshots from your `.docx` output.

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
