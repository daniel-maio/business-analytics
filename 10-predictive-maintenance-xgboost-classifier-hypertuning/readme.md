# IoT Predictive Maintenance Pipeline (Sensor Fault Binary Classification)

Machine Learning pipeline developed to solve **Predictive Maintenance** problem using industrial IoT sensor logs. The system ingests telemetry data from 178 sensors to predict whether the machines require technical intervention.

## Key Features

- Core Machine Learning: `XGBoost (XGBClassifier)`, `scikit-learn` (LogisticRegression)
- Optimization & Benchmarking:** Hyperparameter Tuning via `GridSearchCV` with Stratified Cross-Validation ($K=3$).
- Data Processing Pipeline: Data-split isolation, Random Undersampling (majority class alignment), and Robust Feature Scaling (`StandardScaler`).
- Advanced Analytics: Performance evaluation using ROC-AUC, Precision/Recall trade-off curves, and multi-split validation overlays.

---