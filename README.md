# DATA-MINING.
Datamining and wrangling-cleaning and exploratory analysis of the global  Tech startups 2026 dataset(2500) startups
# Global Technology Startup Success Analysis

## Overview

This project works through the full early-stage data pipeline  sourcing a dataset, cleaning it, exploring it visually, and investigating relationships between variables  using a dataset of global technology startups.

The analysis investigates how funding, revenue, valuation, workforce size, financial runway, investor support, AI adoption, sector, and location relate to the performance and outcomes of technology startups.

## Dataset

- **Source:** [Global Tech Startups 2026 / Startup Success Analysis (Kaggle)](https://www.kaggle.com/code/veynvennie/startup-success-analysis/input)
- **Size:** 25,000 rows × 17 columns
- **Unit of observation:** each row represents one technology startup
- **Variables:** a mix of numerical (funding, valuation, revenue, burn rate, runway, headcount) and categorical (domain, country, funding stage, AI adoption level, acquisition status) fields

## What's in this repo

| File | Description |

| DATAM.ipynb | Jupyter notebook containing the full analysis: data cleaning, exploratory visualization, and relationship analysis, with markdown narrative throughout |
| global_tech_startups_2026.csv` | The raw dataset used for the analysis |

## Project structure (inside the notebook)

1. **Introduction & Dataset Source** — motivation for choosing the dataset and the research questions guiding the analysis
2. **Data Cleaning** — missing value audit and treatment, duplicate/ID checks, zero-value investigation, and outlier detection (IQR method), each with before/after comparisons and justification
3. **Data Visualization & Exploratory Analysis** — distribution of categorical variables (domain, country, outcome) and numerical variables (funding, revenue), with summary statistics and interpretation
4. **Relationships Between Variables** — scatterplots and Pearson correlation coefficients between key financial variables (funding, valuation, revenue), plus a full correlation heatmap across all numerical variables
5. **Major Findings** — summary of key patterns and takeaways from the analysis

## Key findings

- The dataset is heavily concentrated in the United States, with China and India as the next largest groups.
- Financial variables (funding, valuation, revenue, burn rate) are strongly right-skewed — a small number of very large startups pull the mean well above the median.
- Total funding and valuation show a very strong positive correlation (r ≈ 0.945); revenue and valuation are also strongly correlated (r ≈ 0.885). These are associations, not evidence of causation.
- Missing AI adoption data (≈10.4% of records) was retained as an explicit "Not Reported" category rather than deleted, preserving all 25,000 observations.

## How to run

bash
pip install pandas numpy matplotlib seaborn
jupyter notebook DATAM.ipynb


Run all cells top to bottom — the notebook combines code, output, and markdown narrative in one reproducible report.

## Authors

Bwambale Sedrack Bisogho,
