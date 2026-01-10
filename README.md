# International Aid Allocation

## Project Overview

The goal of this notebook is to apply unsupervised learning techniques to identify countries in greatest need of humanitarian assistance. The dataset contains socio-economic and health indicators for 167 countries.

**Dataset Source:** [Kaggle - Unsupervised Learning on Country Data](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data)

## Algorithms Tested

- **K-Means Clustering** (primary method)
- **DBSCAN** (Density-Based Spatial Clustering)
- **Hierarchical Clustering** (Agglomerative with Ward linkage)

## Methodology

After comprehensive Exploratory Data Analysis and feature scaling, multiple clustering algorithms are evaluated using:

- Elbow Method
- Silhouette Analysis
- PCA visualization

The optimal **K=3 clusters** are identified, representing:

1. **Developed Nations** - self-sufficient countries
2. **Developing Nations** - transitional economies requiring targeted support
3. **Underdeveloped Nations** - countries requiring urgent humanitarian intervention

## Key Features

- Correlation analysis of 9 socio-economic indicators
- Distribution analysis and country rankings
- Geographic visualization of cluster distribution
- Strategic budget allocation framework ($10M)
- Comparative performance analysis across algorithms

## Results

K-Means clustering with **K=3** is selected as the optimal solution, achieving a silhouette score of **0.283**. While K=5 shows a marginally higher score (0.299), K=3 is chosen for its superior balance of statistical performance, business interpretability, and operational simplicity. The analysis identifies priority countries and proposes a data-driven budget distribution proportional to need severity, with three clear categories that align with international development classifications.

## Dataset Variables

| Variable | Description |
|----------|-------------|
| `child_mort` | Child mortality rate (deaths per 1000 live births) |
| `life_expec` | Life expectancy at birth (years) |
| `income` | Net income per person (USD) |
| `gdpp` | GDP per capita (USD) |
| `health` | Health spending (% of GDP) |
| `total_fer` | Fertility rate (children per woman) |
| `exports` | Exports (% of GDP) |
| `imports` | Imports (% of GDP) |
| `inflation` | Annual GDP growth rate (%) |

---

*This notebook is part of the Coursera IBM Machine Learning Professional Certificate program.*
