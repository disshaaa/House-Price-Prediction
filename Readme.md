# 🏠 House Price Prediction 

This project aims to predict the **Sale Price of residential homes** using various regression algorithms on the [House prices dataset](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data). The goal is to compare multiple models and evaluate their performance using key regression metrics and visualizations.

---

## 📁 Dataset

**Source**: [House prices Datasets on Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

- **Train data**: 1460 rows × 81 columns
- **Test data**: 1459 rows × 80 columns (without target)

The dataset contains various features like zoning classification, lot size, neighborhood, number of rooms, condition of property, garage details, etc.

---

## ⚙️ Project Workflow

### ✅ Step 1: Data Loading and Inspection
- Loaded train and test CSV files
- Checked for missing values and performed visual + statistical inspections

### ✅ Step 2: Data Preprocessing
- Handled missing values (imputation or removal based on feature)
- Label encoded categorical features using `LabelEncoder`
- Concatenated and split data back into `X_train`, `X_test`, and `y_train`
- Final train shape: `X_train`: (1168, 75), Validation: (292, 75)

### ✅ Step 3: Model Building and Evaluation

#### Regression Models Applied:
1. Simple Linear Regression
2. Multiple Linear Regression
3. Polynomial Regression
4. Ridge Regression
5. Lasso Regression
6. ElasticNet Regression
7. Decision Tree Regressor
8. Support Vector Regressor
9. K-Nearest Neighbors
10. Random Forest Regressor ✅ (Best Model)

### ✅ Step 4: Model Evaluation

Used the following metrics to evaluate performance:
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)
- R² Score (Coefficient of Determination)

📉 Plotted residuals and regression lines for visual insight  
📊 Compared all models using RMSE in a bar chart

---

## 📈 Results

| Model                    | RMSE        |
|--------------------------|-------------|
| Random Forest Regressor  | **28,818** ✅ |
| Simple Linear Regression | 34,156       |
| Multiple Linear Regression | 34,156     |
| Lasso Regression         | 34,156       |
| ElasticNet Regression    | 34,170       |
| Ridge Regression         | 34,176       |
| Decision Tree Regressor  | 39,385       |
| KNN                      | 48,942       |
| SVR                      | 88,619       |
| Polynomial Regression    | 550,472 ⚠️    |

📌 **Best model**: `RandomForestRegressor` with lowest RMSE  
📌 Residuals are tightly clustered, showing good prediction spread

---

## 📊 Visuals Included

- Regression Line plots
- Residual plots
- RMSE bar chart comparison
- Predictions on test set using best model

---

## 📚 Future Enhancements

- Use feature selection or PCA
- Apply advanced models like XGBoost or LightGBM
- Try log-transforming skewed features
- Perform GridSearchCV for hyperparameter tuning

---

## 🧠 Skills Used

- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn: regression models & metrics
- EDA, data cleaning, encoding, splitting
- Regression evaluation & interpretation

---

## 🔗 Dataset Link

👉 [House Prices Dataset - Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

---
