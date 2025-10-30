# 🏠 House Prices – Advanced Regression Techniques

**Author:** Karthikeyan M  

This project predicts house prices based on various property characteristics such as area, quality, year built, and location.  
It is built using the [Kaggle: House Prices – Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset.

---

## 🚀 Project Overview
The goal is to predict the final sale price of homes using advanced regression algorithms.  
The notebook includes end-to-end processing — from data cleaning and feature engineering to model training, evaluation, and visualization.

---

## 📊 Dataset
**Source:** Kaggle  
**Key Features:** `MSSubClass`, `MSZoning`, `LotArea`, `OverallQual`, `YearBuilt`, `GrLivArea`, `GarageCars`, `SalePrice`  
**Target Variable:** `SalePrice`

---

## 🧠 Machine Learning Models Used
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Support Vector Regressor (SVR)

---

## ⚙️ Evaluation Metrics
The models were evaluated using regression and classification-style metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- **ROC–AUC Curve** (for binary threshold classification of predicted prices)

---

## 📈 Model Performance Summary

| Model | R² Score | RMSE | AUC | Remarks |
|-------|----------:|------:|-----:|---------|
| Linear Regression | 0.8807 | 0.197 | — | Baseline linear model |
| Decision Tree | 0.9992 | 0.0316 | **1.000** | ⚠️ Overfit (perfect AUC, unrealistic) |
| Random Forest | 0.9981 | 0.1544 | 0.997 | Strong performer, minor overfit |
| **SVR** | **0.9891** | **0.1154** | **0.999** | ✅ Best balanced model (excellent AUC + generalization) |

> The Decision Tree achieved perfect R² and AUC = 1.000, indicating overfitting to the training data.  
> The **SVR model** achieved nearly perfect AUC (0.999) and high R² (0.989), making it the **best generalizing model overall**.

---

## 🧩 Feature Overview
**Numerical Features:** `OverallQual`, `GrLivArea`, `GarageCars`, `GarageArea`, `TotalBsmtSF`, `1stFlrSF`, `FullBath`, `TotRmsAbvGrd`  
**Categorical Features:** `MSZoning`, `Neighborhood`, `KitchenQual`

---

## 🛠️ Tools & Libraries
- Python 3.9+  
- Pandas | NumPy  
- Matplotlib | Seaborn  
- Scikit-learn  
- Google Colab

---

## 📊 Visualizations
- Correlation heatmaps of numerical features  
- Feature importance bar charts  
- ROC–AUC curve comparison for all models  
- Distribution plots before and after preprocessing  

---

## ▶️ How to Run
1. Open `House_Prices_Advanced_Regression_Techniques.ipynb` in **Google Colab**.  
2. Upload the Kaggle dataset files (`train.csv`, `test.csv`).  
3. Run all cells sequentially.  
4. Review the printed metrics and visualizations at the end for model comparisons.

---

## 🧾 Conclusion
- **Decision Tree** → Overfits (perfect R² and AUC = 1.000)  
- **Random Forest** → High accuracy but slightly less generalization  
- **SVR** → Best overall balance (AUC = 0.999, R² = 0.9891, RMSE = 0.1154)

✅ Final Conclusion: **SVR is the best generalized model** for predicting house prices in this project.

---

## 👨‍💻 Author
**Karthikeyan M**

---
