# Predictive Maintenance Framework for Imbalanced Sensor Data

This repository contains an end-to-end Machine Learning pipeline that targets **Predictive Maintenance** using industrial sensor data. The core objective is to accurately classify whether machinery requires immediate technical intervention while benchmarking techniques to solve extreme **class imbalance** problems.

## Tech Stack & Technical Competencies

- Core Classifier: RandomForestClassifier (scikit-learn)
- Imbalanced Data Engineering: Class Weight Balancing, Undersampling, Oversampling (`sklearn.utils.resample`), and Synthetic Minority Over-sampling Technique (`imblearn.over_sampling.SMOTE`)
- Data Processing: Robust scaling pipeline (`StandardScaler`)
- Evaluation Metrics: Precision, Recall, F1-Score, and ROC-AUC for skewed distributions.

## Quickstart
```bash
pip install numpy pandas scikit-learn imbalanced-learn
```

---