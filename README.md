# 🧪 Diabetes Prediction Classifier

This project builds a binary classification model to predict whether a patient has diabetes based on medical and demographic features.

## 📊 Dataset Description

The dataset includes the following features:
- Age
- Gender
- BMI (Body Mass Index)
- Hypertension
- Heart Disease
- Smoking History
- HbA1c level
- Blood Glucose Level

The target variable is `diabetes`, which is:
- `1` — Positive
- `0` — Negative

## 🎯 Objective

Train a machine learning classifier to accurately predict diabetes status and generate predictions on unseen test data.

## 🚀 Workflow

- Data loading and cleaning
- Exploratory Data Analysis (EDA)
- Feature encoding and scaling
- Model selection and training (RandomForest, XGBoost, etc.)
- Hyperparameter tuning
- Evaluation (accuracy, precision, recall)
- Prediction on test data
- Submission generation

## 📁 Project Structure

```bash
diabetes-classification-project/
│
├── notebooks/
│   └── diabetes_classifier.ipynb         # Main Jupyter notebook with the full solution
│
├── data/
│   ├── training_data.csv                # Training dataset with features and target
│   ├── test_data.csv                    # Test dataset without the target variable
│   └── submission.csv                   # Final predictions in the required format
│
├── README.md                            # Project description and instructions
├── requirements.txt                     # List of required Python packages
└── .gitignore                           # Specifies which files to exclude from version control
```

## ✅ Submission Format

The final submission must be in `.csv` format with two columns:
- `ID`
- `prediction` — a **class label** (0 or 1), not probability


## ⚙️ Setup & Run

To run the notebook:

```bash
pip install -r requirements.txt
export PATH=$PATH:/Users/zsakhipo/Library/Python/3.9/bin
jupyter notebook
jupyter notebook notebooks/diabetes_classifier.ipynb
