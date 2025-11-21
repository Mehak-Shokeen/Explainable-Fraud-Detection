# AI-Powered Explainable Credit Card Fraud Detection
### 🔍 XGBoost • SHAP • SMOTE • PCA Dataset • Web App
A complete end-to-end machine learning system that detects fraudulent credit card transactions with AI explainability.<br>
Built using XGBoost, interpreted with SHAP, balanced with SMOTE, and deployed as a web application for easy use.

## 🚀 Project Overview
This project identifies fraudulent credit card transactions using an AI model and explains why a transaction was marked as fraud.<br>
Since fraud detection is a high-risk domain, adding Explainable AI (XAI) increases trust, transparency, and accountability.

## 📂 Dataset
We used the Credit Card Fraud Detection Dataset from Kaggle.<br>
Key points:<br>
● Contains real European credit card transactions<br>
● Heavily imbalanced (fraud < 1%)<br>
● Features V1–V28 are PCA-transformed for confidentiality<br>
● Class is the target variable<br>
    - 0 → Legitimate<br>
    - 1 → Fraud<br>

## 🧹 Data Preprocessing

● Dropped the Time feature (not useful for prediction)<br>
● Standardized the Amount feature using StandardScaler to match PCA feature scales<br>
● Performed EDA to understand fraud distribution and feature patterns<br>
● Applied SMOTE to handle severe class imbalance<br>
● Split the data into training and testing sets<br>

## 🤖 Model Used: XGBoost

We chose XGBoost because it:<br>
● Handles imbalanced classes well<br>
● Works great with tabular data<br>
● Captures complex, non-linear patterns<br>
● Gives high accuracy and AUC scores

## 🔍 Explainability: SHAP

To avoid “black-box” predictions, we integrated SHAP (SHapley Additive exPlanations).<br>

SHAP provides:<br>
● Feature contribution for each prediction<br>
● Global and local interpretability<br>
● Visual plots explaining why a transaction was flagged<br>

## 📊 Evaluation Metrics

The model was evaluated using:<br>
Accuracy (99.5%)<br>
Precision (91%), Recall(82%), F1-score<br>
ROC-AUC<br>
Confusion Matrix<br>

Because of class imbalance, AUC and Recall were prioritized.

## 🛠️ Tech Stack<br>

● Python<br>
● Pandas, NumPy<br>
● XGBoost<br>
● Scikit-learn<br>
● SHAP<br>
● Imbalanced-Learn (SMOTE)<br>

## 👥 Team Contribution Note

This project was completed as a team effort. I personally handled the data preparation workflow, including data collection, preprocessing, dropping irrelevant attributes, SMOTE for balancing, feature scaling and the entire EDA process. The web integration and deployment module is currently in progress as part of the ongoing collaborative development.
