# ADS502-FINAL-PROJECT
# Clustering Medicare Prescribers to Identify High-Risk Prescribing Patterns

## Overview
This project uses the Medicare Part D Prescribers by Provider 2023 dataset 
to identify patterns in opioid prescribing behavior through unsupervised 
clustering. The goal was to explore whether prescribers could be grouped by 
behavioral patterns that might indicate elevated opioid prescribing risk.

## Team
- **Jacob H.** — Data cleaning and exploratory data analysis
- **Megan L.** — Data modeling (K-Prototypes and K-Means clustering)
- **Julia G.** — Results analysis and performance evaluation

## Dataset
Medicare Part D Prescribers by Provider 2023 — Centers for Medicare & 
Medicaid Services (CMS)
- 1,380,665 rows, 84 features
- Dataset not included due to file size
- Available at: https://data.cms.gov/provider-summary-by-type-of-service/medicare-part-d-prescribers/medicare-part-d-prescribers-by-provider/data

## Repository Structure
- `main` branch — `FINAL_PROJECT_ADS502_GROUP3.ipynb` — full project 
  notebook including data cleaning, modeling, and results analysis
- `Jacob` branch — `data-cleaning-jacobh.ipynb` — Jacob's data cleaning 
  and EDA notebook
- `mlee_ads502` branch — Megan's modeling notebooks
- `julia_results` branch — Julia's results analysis drafts
- `archive` branch — previous working versions of the combined notebook

## How to Run
1. Download the 2023 CSV from the CMS link above
2. Place it in the same folder as the notebook
3. Run all cells from top to bottom

## Requirements
- pandas
- numpy
- scikit-learn
- kmodes
- matplotlib
- seaborn
- plotnine
- scipy
- statsmodels

## Key Findings
- A consistent group of 19 extreme outlier providers surfaced across 
  multiple subgroups
- Pain management providers prescribed opioids at over 27 times the rate 
  of all other providers
- The dataset skews heavily toward lower volume prescribers which 
  influenced cluster size distributions

## Limitations
- Silhouette scoring was not feasible on the full dataset due to 
  computational constraints
- Patient level data such as outcomes and diagnosis codes would be needed 
  to confirm high risk classification
- The dataset is limited to Medicare Part D and may not capture the full 
  picture of opioid prescribing
