# 🕵️‍♂️ Credit Card Fraud Detection with XGBoost, SHAP & Power BI

A complete machine learning pipeline to detect fraudulent credit card transactions using real-world class-imbalanced data, SHAP for model explainability, and Power BI for business visualization.  
Developed as part of my portfolio to demonstrate applied ML, interpretability, and data storytelling skills for risk analytics roles.

---

## 📌 Problem Statement

Credit card fraud is a significant issue in the financial industry, especially due to the rarity and unpredictability of fraudulent transactions. The goal is to build a robust classification model that can:

- Accurately flag fraudulent transactions
- Handle extreme class imbalance
- Provide explainable results for business trust
- Present results interactively for stakeholders

---

## 🧠 Technologies Used

- **Python**: pandas, scikit-learn, XGBoost, SHAP
- **Modeling Techniques**: SMOTE resampling, Logistic Regression, XGBoost
- **Explainability**: SHAP (TreeExplainer, summary plots)
- **Evaluation Metrics**: F1-score, Recall, Confusion Matrix
- **Visualization**: Power BI, matplotlib, seaborn

---

## ⚙️ Project Workflow

1. **Data Exploration & Preprocessing**  
   - Loaded dataset (`transactions.csv`)
   - Handled severe class imbalance (0.17% fraud) using SMOTE
   - Scaled features (StandardScaler) and split into train/test sets

2. **Model Training & Evaluation**  
   - Trained XGBoost classifier  
   - Achieved recall of **85%** and **F1-score of 0.88** on fraud class  
   - Compared with Logistic Regression baseline

3. **Model Explainability**  
   - Applied SHAP to understand feature influence  
   - Identified `V14`, `V4`, and `V12` as top fraud indicators

4. **Export & Visualization**  
   - Exported predictions to `results.csv`  
   - Built a Power BI dashboard to visualize fraud detection outcomes

---

## 📁 Repository Structure

```
├── README.md
├── requirements.txt
├── data/
│   └── results.csv
├── notebooks/
│   └── fraud_model.ipynb
├── dashboard/
│   └── PowerBI.pbix
├── images/
│   └── dashboard.png
```

---

## 📌 Key Results

- **Recall on fraud class**: 0.85  
- **F1-score**: 0.88  
- **Explainable AI (SHAP)** used for model transparency  
- Designed for real-world interpretability and business use
