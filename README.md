# 🛒 SmartCart Customer Segmentation

*Unsupervised ML for E-commerce Marketing Strategy*

## Problem Statement

SmartCart, a growing e-commerce platform, currently uses generic marketing strategies for all customers — resulting in wasted budget, missed opportunities, and poor retention.

**Goal:** Use unsupervised machine learning to discover hidden customer segments from behavioral and demographic data, and translate those segments into actionable marketing strategies.

## Dataset

- 2,240 customer records, 22 attributes
- Covers demographics, purchase behaviour, and campaign response
- Source: Customer Personality Analysis (Kaggle / UCI)

## Approach

1. Data Cleaning & Missing Value Treatment
2. Feature Engineering
3. Outlier Detection & Removal
4. EDA & Correlation Analysis
5. Feature Encoding & Scaling
6. Dimensionality Reduction (PCA)
7. Clustering — K-Means & Agglomerative Clustering
8. Cluster Profiling & Business Insights

### Model Selection Note

K-Means was tested first using the elbow method and silhouette score, but produced poorly separated clusters. Agglomerative Clustering gave significantly better-defined, more interpretable segments and was used for the final analysis.

## Key Result — 4 Customer Segments

| Segment | Avg Income | Avg Spending | Campaign Response | Strategy |
|---|---|---|---|---|
| Family Shoppers (price sensitive) | $39,680 | $222 | 7.6% | Discount campaigns |
| Loyal Affluent Families | $72,808 | $1,236 | 16.7% | Loyalty programs |
| Digital Browsers (budget singles) | $36,960 | $165 | 14.2% | Web flash sales |
| High Value Singles (best ROI) | $70,722 | $1,190 | 32.0% | Premium services |

### Strategic Insight

"Loyal Affluent Families" and "High Value Singles" share nearly identical income and spending — but differ in household structure (couples vs. singles). Same product, different messaging: family/shared value vs. personal indulgence — a clear example of how clustering enables precision marketing beyond simple demographics.

## Tech Stack

`Python` `Pandas` `NumPy` `Scikit-learn` `Seaborn` `Matplotlib` — PCA, K-Means, Agglomerative Clustering, Elbow Method, Silhouette Score

## How to Run

```bash
git clone https://github.com/Khyatisinha25/smartcart-customer-segmentation.git
cd smartcart-customer-segmentation
jupyter notebook smartcart_clustering.ipynb
```

## Author

**Khyati Sinha** — [GitHub](https://github.com/Khyatisinha25) · [LinkedIn](https://www.linkedin.com/in/khyati-sinha2510/)

