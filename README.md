# AI Risk Forecasting System

## Extended Description
The AI Risk Forecasting System is a Python-based machine learning project designed to predict the probability of loan default and classify borrowers into risk levels: HIGH, MEDIUM, or LOW. 

The system leverages **Logistic Regression**, along with data preprocessing techniques like feature scaling and train-test splitting. It demonstrates the full ML workflow: loading and inspecting data, preparing features and labels, training a model, evaluating performance, and producing actionable predictions.

This project is modular and extensible, with separate folders for Python ML scripts (`python_ml`), a potential C engine integration (`c_engine`), and sample datasets (`data`). Anyone can clone the repository, install dependencies, and run predictions easily.

## Folder Structure
AI_Risk_Forecasting_System/
├── python_ml/ # Python ML scripts
│ └── ml_csv_test.py
├── c_engine/ # C engine scripts (optional integration)
├── data/ # Sample data files
│ └── sample.csv
└── README.md # This file

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
- Accuracy is low due to the small sample dataset.
- Warnings about `feature names` are safe and do not affect predictions.

## Skills Demonstrated
- Data Analysis with Pandas
- Logistic Regression with Scikit-Learn
- Data Scaling & Train-Test Split
- Risk Assessment Logic
- Git & GitHub Version Control

