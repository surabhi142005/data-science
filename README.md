project/
├── data/
│   └── tested.csv
├── notebooks/
│   └── exploration.ipynb
├── src/
│   ├── __init__.py
│   ├── preprocess.py
│   ├── train_model.py
│   └── evaluate.py
├── requirements.txt
└── README.md

# src/preprocess.py
[from previous content...]

# src/train_model.py
[from previous content...]

# src/evaluate.py
[from previous content...]

# requirements.txt
pandas
scikit-learn

# README.md
# Titanic Survival Prediction

This project builds a machine learning model to predict survival on the Titanic using passenger data.

## 📁 Project Structure
```
project/
├── data/              # Dataset location
├── notebooks/         # For EDA and experimentation
├── src/               # Source code
│   ├── preprocess.py  # Preprocessing pipeline
│   ├── train_model.py # Model training
│   └── evaluate.py    # Evaluation metrics
├── requirements.txt   # Project dependencies
└── README.md          # Project overview
```

## ⚙️ Setup
```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## 🚀 Usage
```bash
# Run training
python src/train_model.py
```

## ✅ Features
- Handles missing values using median imputation
- Extracts and encodes titles from names
- One-hot encodes categorical variables
- Scales numerical features
- Compares Logistic Regression and Random Forest

## 📊 Evaluation Metrics
Each model prints out:
- Accuracy
- Precision
- Recall
- F1 Score
- Full classification report

## 📦 Requirements
```txt
pandas
scikit-learn
```

## 📈 Example Output
```
Random Forest Performance:
              precision    recall  f1-score   support

           0       0.87      0.90      0.88       105
           1       0.83      0.78      0.80        74

    accuracy                           0.85       179
   macro avg       0.85      0.84      0.84       179
weighted avg       0.85      0.85      0.85       179
```
