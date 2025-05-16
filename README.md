# 🏡 Airbnb Price Prediction - San Diego

This project analyzes Airbnb listing data in San Diego to identify factors that influence rental price. Using SAS, we perform data cleaning, regression modeling, and machine learning to build predictive models and compare performance.

## 📌 Objective
To build a model that predicts Airbnb prices based on features like room type, number of beds, availability, and review scores using linear regression, decision tree, and random forest models.

---

## 🧰 Tools & Technologies
- **Language:** SAS
- **Procedures Used:** `PROC IMPORT`, `PROC UNIVARIATE`, `PROC GLMSELECT`, `PROC HPSPLIT`, `PROC HPFOREST`
- **Model Types:** Linear Regression, LASSO, Decision Tree, Random Forest

---

## 🗂️ Project Structure

| Folder        | Content |
|---------------|---------|
| `code/`       | All SAS scripts for data import, preprocessing, and modeling |
| `data/`       | Airbnb listings dataset (sample) |
| `visuals/`    | Exported charts and visualizations (optional) |
| `report/`     | Final project report as PDF |
| `README.md`   | Overview of the project |

---

## 📊 Key Analysis Steps

- Imported Airbnb data and cleaned missing or skewed values
- Investigated outliers and distribution of the `price` variable using `PROC UNIVARIATE`
- Applied transformations (e.g., log-price) where needed
- Checked for multicollinearity using correlation matrices and VIF
- Collapsed high-cardinality categorical variables where necessary
- Split data into training and testing sets (80/20)
- Built regression models using `PROC GLMSELECT` with LASSO
- Built a decision tree using `PROC HPSPLIT`
- Built a random forest using `PROC HPFOREST`
- Compared model performance based on RMSE on both train/test sets

---

## 📈 Results & Recommendations

- **Regression Model**: Baseline model, interpretable but limited in performance
- **Decision Tree**: Improved model interpretability with moderate performance gain
- **Random Forest**: Best RMSE on both train and test data

✅ **Recommendation**: Random Forest provides the best performance and should be considered for deployment.

---

## 🚀 How to Run

> All code is written in SAS and structured for modular execution.

- Open `code/import_cleaning.sas` to import and clean the data
- Use `regression_modeling.sas` for LASSO model building
- Use `decision_tree.sas` and `random_forest.sas` to build and evaluate machine learning models
- View `report/SAS_project_SanDiego.pdf` for summary and results

---


