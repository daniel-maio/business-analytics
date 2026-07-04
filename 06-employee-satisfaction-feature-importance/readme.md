# Employee Attrition Pipeline

A Machine Learning and Data Engineering pipeline designed to identify, process, and predict the structural organizational factors that explain employee turnover and attrition risks.

## Key Features

- Target Filtering and Mapping: Filters categorical records to focus explicitly on active versus voluntarily resigned personnel profiles. It converts the text-based classes into a clean binary classification state (0 for Current employee, 1 for Voluntary Resignation).
- Parallel Feature Pre-processing: Splits columns into distinct numerical and categorical channels using automated data type selectors.
- Numerical Architecture: Chains a data imputation layer utilizing median values with a standard Z-score data scaling execution layer (`StandardScaler`).
- Categorical Architecture: Implements a text-handling fallback layer that assigns missing entries to a constant state, followed by an optimized `OneHotEncoder` configuration to bypass unknown category exceptions during test steps.
- Unified Column Transformers: Merges parallel pipelines into a unified data engineering structure (`ColumnTransformer`) to process rows simultaneously.
- Linear Inference & Feature Importance: Encapsulates the operations inside a master pipeline containing a `LogisticRegression` classifier. The script extracts log-odds layer weights (`coef_`) alongside dynamically tracked feature column names (`get_feature_names_out`) to rank statistical indicators.

## Quick Start
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

---