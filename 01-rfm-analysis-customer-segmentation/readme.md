# E-Commerce Customer Segmentation Pipeline (RFM Analysis)

This repository contains a production-ready data science pipeline that implements **RFM (Recency, Frequency, Monetary)** analysis to segment an e-commerce customer base. The project processes raw transaction history, engineers behavior-based features, clusters profiles into tactical marketing categories, and outputs an interactive business dashboard.

## Key Features
- Data Manipulation: `pandas`, `numpy`
- Feature Engineering: Custom quantile discretization (`pd.qcut`), percentile-rank processing, and multi-variable aggregation.
- Data Visualization: `plotly.graph_objects` (Interactive Treemaps), `seaborn`, `matplotlib`
- Business Intelligence: Data-driven marketing automation rules and customer profile indexing.

## Quickstart

```bash
pip install pandas seaborn plotly matplotlib scikit-learn
```
---