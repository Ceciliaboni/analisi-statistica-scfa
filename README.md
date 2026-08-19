# Statistical Analysis of Short-Chain Fatty Acids (SCFAs)

### Multi-disease study on parallel plasma and fecal samples

This repository contains the statistical analysis developed for my Bachelor's thesis in Statistics at the University of Florence during the Academic Year 2024/2025.

The study investigates the concentrations of seven short-chain fatty acids (SCFAs) measured in plasma and fecal samples from four clinical groups.

The main objectives are to:

- compare SCFA concentrations across clinical groups;
- evaluate their ability to discriminate between different clinical conditions;
- investigate the relationship between plasma and fecal SCFA concentrations.

---

## Clinical Groups

The analysis considers four clinical groups:

- **CD** — Celiac Disease
- **CRC** — Colorectal Cancer
- **HC** — Healthy Controls
- **Obesi** — Obesity

For each patient, the concentrations of seven SCFAs were measured in both plasma and fecal samples.

---

## Statistical Methods

The analysis includes:

- Descriptive statistics
- Correlation analysis
- Principal Component Analysis (PCA)
- Hierarchical Cluster Analysis
- Ward's method
- Kruskal-Wallis test
- Dunn's post-hoc test
- Multinomial Logistic Regression
- 10-fold Cross-Validation
- Fisher's Linear Discriminant Analysis (LDA)

These methods were used to investigate differences between clinical groups and evaluate the discriminatory ability of SCFA concentrations.

---

## Key Findings

The analysis shows that **plasma SCFA concentrations are more informative than fecal concentrations for discriminating between the clinical groups**.

In particular, plasma measurements provide stronger discrimination of healthy controls from the clinical groups.

The multinomial logistic regression analysis also identifies **Valeric acid** as consistently associated with clinical group membership in the plasma data.

The combined plasma and fecal model provides good classification results, but does not show a substantial improvement compared with the plasma model alone.

The hierarchical clustering analysis based on Ward's method does not fully separate all four clinical groups, although plasma and fecal samples appear to provide complementary information.

---

## Analysis Workflow

```text
Data
 │
 ├── Plasma samples
 │
 └── Fecal samples
        │
        ▼
Exploratory Analysis
        │
        ├── Descriptive statistics
        ├── Correlations
        └── PCA
        │
        ▼
Cluster Analysis
   └── Ward's method
        │
        ▼
Group Comparison
   ├── Kruskal-Wallis
   └── Dunn's test
        │
        ▼
Multinomial Logistic Regression
   ├── Plasma
   ├── Fecal
   └── Combined data
        │
        ▼
10-Fold Cross-Validation
        │
        ▼
Classification
   └── Fisher's LDA
```
## Technologies

The analysis was developed in **R**.

The main statistical methods and topics covered in the project are:

- Statistical inference
- Exploratory data analysis
- Multivariate analysis
- Principal Component Analysis (PCA)
- Cluster analysis
- Classification
- Logistic regression
- Linear Discriminant Analysis (LDA)
- Cross-validation
- Data visualization

---

## Repository Structure
```text
.
├── README.md
├── tesi.R
└── tesi.pdf
```
- ```tesi.R``` — R script containing the statistical analyses.
- ```tesi.pdf``` — Bachelor's thesis.
- ```README.md``` — project documentation.
---
## Academic Context

**Bachelor's Degree in Statistics**
University of Florence
School of Economics and Management

**Academic Year**: 2024/2025

**Thesis title**:

*Un'analisi statistica degli acidi grassi a catena corta: studio multi-malattia su due campioni paralleli*

**Supervisor**: Prof. Francesco Claudio Stingo

**Author**: Cecilia Boni
