# ❤️ Heart Disease Prediction (Clinical Classification)

This project focuses on predicting the presence of heart disease in patients using various physiological factors. The primary goal was to build a model that prioritizes **patient safety** by maximizing **Recall** (minimizing missed cases).

## 📊 Key Findings & Metrics
In medical diagnostics, missing a sick patient (False Negative) is more critical than a false alarm. Therefore, the models were evaluated based on their ability to capture all "Presence" cases.

| Model | Accuracy | Recall (Class: Presence) |
| :--- | :---: | :---: |
| **Logistic Regression** | 85% | **86% (Best)** |
| Random Forest | 81% | 76% |
| XGBoost | 83% | 71% |

**Why Logistic Regression?** Despite being a simpler model, it provided the highest Recall for diseased patients in this dataset, making it the most reliable choice for initial clinical screening.

## 🛠️ Tech Stack & Methods
- **Preprocessing:** Standard scaling for numerical features and label encoding for the target.
- **Algorithms:** Logistic Regression, Random Forest, and XGBoost.
- **Handling Imbalance:** Utilized `class_weight='balanced'` to ensure the model focuses on detecting heart disease cases equally.

## 🔍 Feature Importance
According to our XGBoost analysis, the most critical factors for diagnosis are:
1. **Chest Pain Type:** The strongest clinical indicator.
2. **ST Depression:** Significant predictor of heart stress.
3. **Thallium Stress Test results.**

## 🚀 How to Use
1. Clone the repo.
2. Install requirements: `pip install pandas scikit-learn matplotlib xgboost`.
3. Run `Heart_Disease_Prediction_task.ipynb` to see the full analysis.
