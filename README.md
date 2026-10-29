# Customer Churn Prediction & Analytics

A machine-learning project that explores customer churn patterns and compares classification models on the Telco customer churn dataset.

## Project overview

The notebook analyzes 7,043 customer records and performs exploratory data analysis, data cleaning, feature preprocessing, statistical association tests, and classification-model evaluation.

## What this project covers

- Exploratory data analysis (EDA), including churn distribution and churn patterns by contract type, tenure, monthly charges, internet service, tech support, and payment method.
- Data preparation, including removal of selected identifier/leakage-related columns, encoding of categorical variables, and scaling of numerical variables.
- Statistical analysis using chi-square tests for selected categorical features.
- Model training and comparison using Logistic Regression, class-weighted Logistic Regression, Random Forest, and XGBoost.
- Evaluation using accuracy, precision, recall, F1-score, and ROC-AUC.
- Experiments with decision-threshold tuning, cross-validation, hyperparameter search, and a stacking classifier.

## Repository structure

```text
customer-churn-prediction/
├── data/
│   ├── README.md
│   └── Telco_customer_churn.xlsx   # Add this dataset file locally
├── project.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Dataset setup

Place `Telco_customer_churn.xlsx` inside the `data/` directory before running the notebook.

The notebook expects this relative path:

```python
data/Telco_customer_churn.xlsx
```

If the dataset is not yours to redistribute or its source license does not permit redistribution, do not commit the Excel file. Instead, add the original dataset source and download instructions here.

## Setup and run

Python 3.10 or 3.11 is a reasonable starting point for this project.

1. Clone the repository.
2. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Add the dataset to `data/Telco_customer_churn.xlsx`.
4. Open `project.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
5. Run the notebook cells in order.

## Models evaluated

- Logistic Regression
- Class-weighted Logistic Regression
- Random Forest
- XGBoost
- Stacking classifier experiment

The notebook also contains threshold-tuning, cross-validation, and hyperparameter-search experiments.

## Evaluation metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Use the outputs produced by the notebook when reporting final model performance. Results can vary with preprocessing, threshold choice, and model configuration.

## Tools and technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Jupyter Notebook and Excel.

## Notes

- Run the notebook from the repository root so the relative dataset path resolves correctly.
- Review the notebook outputs and remove any exploratory/debugging cells that are not needed before presenting the project publicly.
- Do not claim a model is the best unless the final, comparable evaluation results support that conclusion.
