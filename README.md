# Addressing Educational Inequities and Multidimensional Marginalization in Pakistan  
### A Data-Driven, Policy-Relevant Empirical Study

---

## Overview

This repository contains the complete research artefacts for a peer-reviewed empirical study investigating **educational inequities, social marginalization, and structural deprivation across Pakistan** using large-scale household and provincial indicators. The work integrates **statistical data engineering, multivariate analysis, dimensionality reduction, and unsupervised learning** to identify latent patterns of disadvantage and to provide evidence-based insights relevant to education policy, social development, and regional planning.

The project is designed and structured as a **reproducible research pipeline**, from raw data ingestion to analytical modeling and visualization, meeting the standards expected in doctoral-level research and international academic publication.

---

## Research Objectives

- Construct a **harmonized, province- and district-level indicator dataset** from heterogeneous national survey sources.
- Quantify **educational access and deprivation** in relation to health, infrastructure, sanitation, and socioeconomic indicators.
- Identify **latent dimensions of marginalization** using Principal Component Analysis (PCA).
- Discover **structural groupings of indicators** via unsupervised clustering to reveal systemic inequities.
- Provide a **transparent, reproducible analytical framework** suitable for policy analysis and academic extension.

---

## Repository Structure

Paper1/
│
├── Dataset/
│ ├── PSLM .csv # Raw indicator-wise datasets (education, health, water, sanitation, etc.)
│ ├── master_transposed.csv # Aggregated intermediate dataset
│ ├── formatted.csv # Reshaped dataset (indicators × provinces)
│ └── finalized.csv # Cleaned, analysis-ready dataset
│
├── Model/
│ └── ResearchworkClustering.ipynb # Full analytical pipeline (EDA → PCA → Clustering → Visualization)
│
├── Supporting Files/
│ ├── Policy documents and tables # Government reports and contextual references
│ ├── Draft manuscripts (DOCX/PDF) # Publication drafts and supporting academic material
│
├── Addressing_Educational_Inequities_and_Marginalization_.zip
│ └── Submission-ready manuscript package
│
└── Paper1Maryam&Soban.zip
└── Co-author consolidated materials


---

## Dataset Description

The study uses indicators primarily derived from **Pakistan Social and Living Standards Measurement (PSLM)** surveys and related national sources. Key domains include:

- **Education**: Literacy rates, school attendance, provincial and district-level access.
- **Health**: Immunization coverage, functional limitations, health indices.
- **Infrastructure & Utilities**: Electricity, sanitation, drinking water sources.
- **Living Conditions**: Toilet facilities, waste management, housing services.

All datasets are merged, cleaned, transposed, and standardized to ensure **cross-indicator comparability**.

---

## Methodological Framework

### 1. Data Engineering
- Automated ingestion and sorting of multiple CSV sources.
- Column-wise and row-wise normalization.
- Missing-value screening and structural consistency checks.

### 2. Feature Scaling
- Z-score normalization across indicators.
- Province-wise and indicator-wise scaling for robustness.

### 3. Dimensionality Reduction
- **Principal Component Analysis (PCA)** to:
  - Identify dominant latent dimensions of deprivation.
  - Reduce noise and multicollinearity.
  - Interpret socio-educational gradients via component loadings.

### 4. Unsupervised Learning
- **K-Means Clustering** with silhouette-based model selection.
- **Hierarchical (Ward) Clustering** for structural validation.
- Cluster-level aggregation and interpretability analysis.

### 5. Visualization & Interpretation
- Scree plots, PCA projections, heatmaps, dendrograms.
- Cluster-wise indicator summaries to support policy narratives.

---

## Key Outputs

- `finalized.csv` – Fully processed dataset ready for downstream analysis.
- PCA loadings and explained variance ratios.
- Indicator clusters revealing structural patterns of marginalization.
- High-resolution figures suitable for academic publication.
- Reproducible Jupyter notebook implementing the complete workflow.

---

## Reproducibility

All analyses are implemented using open-source Python libraries:

- `pandas`, `numpy`, `scikit-learn`
- `matplotlib`, `seaborn`
- `scipy`

The notebook is fully executable and can be extended for:
- Temporal analysis
- Policy simulations
- Integration with econometric or causal models

---

## Academic Contribution

This work provides:
- A **methodologically rigorous framework** for studying educational inequities in developing contexts.
- A **scalable analytical pipeline** applicable to other countries and survey systems.
- Empirical evidence linking education outcomes with multidimensional deprivation.
- A foundation for **doctoral research extensions**, including causal inference, longitudinal modeling, and policy evaluation.

---

## Citation & Use

This repository accompanies a formal academic publication.  
If you use or extend this work, please cite the corresponding paper and acknowledge the authors.

---

## Authors

**Maryam Arif**  
**Soban Saeed**  

Research domains:  
Education Policy · Social Inequality · Data Science · Applied Machine Learning · Development Studies

---

## License

This repository is released for **academic and research use**.  
Commercial use requires explicit permission from the authors.

---

*This repository represents a complete, publication-grade research artefact designed for scholarly review, replication, and extension.*
