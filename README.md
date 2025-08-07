# Exposure to Air Pollutants and Heart Failure Incidence

**Author:** Madison Morales  
**Institution:** Brandeis University – RBIF 120 Research Topics in Computational Biology  
**Advisor:** Dr. Karol Estrada  
**Date:** June 16, 2025

---

## Overview

This research project explores the interaction between air pollution exposure, genetic risk, and heart failure incidence using UK Biobank data. By integrating environmental data (e.g., PM₂.₅, NO₂, NOₓ), polygenic risk scores (PRS), and proteomic biomarkers (IL-6, SOD1, SOD2), the study aims to uncover how these factors interact biologically and statistically to influence cardiovascular outcomes.

---

## Objectives

1. Assess whether air pollution exposure (PM₂.₅, NO₂, NOₓ) is associated with heart failure.
2. Evaluate whether genetic susceptibility (PRS) modifies these associations.
3. Examine whether proteomic markers (IL-6, SOD1, SOD2) mediate or interact with pollution effects.
4. Account for genetic ancestry using principal component analysis (PCA).

---

## Data Sources

- **UK Biobank** cohort (n ≈ 500,000).
- Air pollution exposure: ESCAPE Land Use Regression (LUR) model.
- Genetic data: PRS computed using PRSice-2 and GWAS summary statistics.
- Proteomic data: Olink Explore 3000 panel.

---

## Statistical Methods

- Logistic and linear regression (base, stepwise, interaction models).
- Variance Inflation Factor (VIF) for collinearity diagnostics.
- Stratified analysis by PRS tertile.
- Principal Component Adjustment for ancestry.

---

## Key Results

- **Pollutant associations (unadjusted)**: PM₂.₅ and NOₓ were positively associated; NO₂ inversely.
- **PRS effect**: Strong and consistent across all models (p < 2e-16).
- **Gene–environment interaction**: All interactions (e.g., PM₂.₅ × PRS) significant.
- **Proteomic biomarker IL-6**: Strong predictor (p < 0.001), even when adjusting for PCs.
- **Adjustment for PCs**: Diminished pollution effects; PRS and IL-6 remained significant.

---

## Repository Structure

| File | Description |
|------|-------------|
| `Exposure to Air Pollutants and Heart Failure Incidence.html` | Full write-up and integrated results |
| `data_exploration.html` | Data cleaning and initial visualization |
| `logistic_regression.html` | Regression model outputs |
| `PCA_models-2.html` | Results including PCA adjustment |
| `PRS_no_proteomics.html` | Models using PRS only |
| `PRS_with_proteomics.html` | PRS + Proteomics interaction results |
| `merge_datasets.index.html` | Merging and preprocessing datasets |

---

### 🔗 View HTML Reports via GitHub Pages

Explore the outputs of this project directly in your browser:

- [Data Exploration](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/data_exploration.html)
- [Logistic Regression Models](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/logistic_regression.html)
- [PRS + Proteomics Analysis](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/PRS_with_proteomics.html)
- [PRS without Proteomics](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/PRS_no_proteomics.html)
- [PCA Models](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/PCA_models-2.html)
- [Dataset Merging Steps](https://mad92morales.github.io/Exposure-to-Air-Pollutants-and-Heart-Failure-Incidence/merge_datasets.index.html)

> All pages are rendered using [GitHub Pages](https://pages.github.com/). If a link doesn’t load immediately, try refreshing — it may still be caching changes.

---

## Tools & Packages

- R packages: `ggplot2`, `knitr`, `tidyr`, `broom`
- PRS generation: `PRSice-2`
- Data transformations: log normalization, rank-inverse normalization

---

## Limitations

- Source code unavailable (hosted on a private cloud).
- Models not fully reproducible without raw datasets.

---

## License

This project does not currently include a license. Please contact the author for reuse or collaboration inquiries.

---

## References

See full list of references in the HTML summary file or contact for PDF.

---
