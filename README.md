# AI Risk Forecasting System

## Extended Description
The AI Risk Forecasting System is a Python-based machine learning project designed to predict the probability of loan default and classify borrowers into risk levels: HIGH, MEDIUM, or LOW. 

The system leverages **Logistic Regression**, along with data preprocessing techniques like feature scaling and train-test splitting. It demonstrates the full ML workflow: loading and inspecting data, preparing features and labels, training a model, evaluating performance, and producing actionable predictions.

This project is modular and extensible, with separate folders for Python ML scripts (`python_ml`), a potential C engine integration (`c_engine`), and sample datasets (`data`). Anyone can clone the repository, install dependencies, and run predictions easily.

## Folder Structure
'''AI_Risk_Forecasting_System/
├── python_ml/ # Python ML scripts
│ └── ml_csv_test.py
├── c_engine/ # C engine scripts (optional integration)
├── data/ # Sample data files
│ └── sample.csv
└── README.md # This file'''

--

## Requirements
- Python 3.x
- pandas
- scikit-learn

## How to Run
1. Clone the repository:
[git clone https://github.com/Ujwala123/AI_Risk_Forecasting_System.git](https://github.com/Anjalinade/AI_Risk_Forecasting_System.git)

--

2. Navigate to the project folder:
cd AI_Risk_Forecasting_System

--

3. Install dependencies:
pip install pandas scikit-learn

4. Run the ML script:
python python_ml/ml_csv_test.py

--


---

## Key Code Snippets

### Data Handling (Pandas & NumPy)
```python
import pandas as pd

data = pd.read_csv("data/sample.csv")
print(data.head())
print(data.describe())

--

#machine learning model (scikit-learn)

from sklearn.linear_model import LogisticRegression
model = LogisticRegression()
model.fit(X_train, y_train)

risk_probability = model.predict_proba(test_case_scaled)[0][1]
print("Risk Probability:", risk_probability)

--

#risk level logic
if risk_probability >= 0.7:
    risk_level = "HIGH"
elif risk_probability >= 0.4:
    risk_level = "MEDIUM"
else:
    risk_level = "LOW"

print("Risk Level:", risk_level)

--

#data visualization
import matplotlib.pyplot as plt

data['loan_amount'].hist()
plt.title("Loan Amount Distribution")
plt.xlabel("Loan Amount")
plt.ylabel("Frequency")
plt.show()

--

## Sample Output
Columns: ['loan_amount', 'income', 'default']

Default column distribution:
0 3
1 3

Model trained successfully
Model Accuracy: 0.5

Confusion Matrix:
[[1 0]
[1 0]]

Classification Report:
precision recall f1-score support
0 0.50 1.00 0.67 1
1 0.00 0.00 0.00 1

Risk Probability: 0.9519385904669366
Risk Level: HIGH

---

## Notes
- Model accuracy is low due to an intentionally small sample dataset used for demonstration.
- The goal of this project is to showcase the end-to-end ML pipeline, not production-grade performance.
- Scikit-learn warning about feature names is expected when using NumPy arrays for prediction and does not affect results.



## Skills Demonstrated
- Data Analysis with Pandas
- Logistic Regression with Scikit-Learn
- Data Scaling & Train-Test Split
- Risk Assessment Logic
- Git & GitHub Version Control

