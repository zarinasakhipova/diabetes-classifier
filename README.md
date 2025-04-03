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
- Model selection and training (RandomForest)
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

## Model Performance 
![Model Performaance](images/model_performance.jpg)

The model used for this Diabetes Classifier project was a Random Forest Classifier, trained on preprocessed patient data. It achieved an accuracy of 96.8% on the test set, showing excellent overall performance.

The results show:
- High precision and F1-score for non-diabetic patients, meaning the model is very accurate when predicting that a person does not have diabetes.
- Slightly lower recall for diabetic patients, which indicates the model missed some true positive cases — a common trade-off in imbalanced medical datasets.
- Despite this, the model maintains a strong overall balance, with a macro F1-score of 0.89 and a weighted F1-score of 0.97, making it reliable for practical use.

These results were achieved through:
- Careful preprocessing (label encoding, scaling)
- Splitting data into training and testing sets
- Training a well-tuned Random Forest model
The model is now capable of making confident predictions on new, unseen patients.

## ✅ Submission Format

The final submission is in `.csv` format with two columns:
- `ID`
- `prediction` — a **class label** (0 or 1), not probability


## ⚙️ Setup & Run

To run the notebook:

```bash
pip install -r requirements.txt
export PATH=$PATH:/Users/zsakhipo/Library/Python/3.9/bin
jupyter notebook
jupyter notebook notebooks/diabetes_classifier.ipynb
