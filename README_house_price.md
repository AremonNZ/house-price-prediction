# 🏠 House Price Prediction — Regression Analysis

A machine learning project that predicts residential property sale prices using the Ames Housing dataset. The goal is to identify the key drivers of house prices and compare the performance of multiple regression models.

---

## 📌 Problem Statement

What makes a house worth more than another? This project explores that question by analysing 1,460 residential property sales across 16 features — from overall quality and living area to neighbourhood and garage size — and building models that can accurately predict sale price.

---

## 📂 Dataset

- **Source:** Ames Housing Dataset
- **Size:** 1,460 rows × 17 columns
- **Target variable:** `SalePrice` (USD)
- **Key features:** Overall quality, above-ground living area, garage capacity, basement size, year built, number of bathrooms, neighbourhood, and more

---

## 🔧 Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas & NumPy | Data manipulation |
| Matplotlib & Seaborn | Data visualisation |
| Scikit-learn | Machine learning models |
| Jupyter Notebook | Development environment |

---

## 🚀 Project Workflow

1. **Data Loading & Overview** — explored shape, data types, and summary statistics
2. **Missing Value Handling** — imputed numeric columns with median, categorical with mode
3. **Exploratory Data Analysis (EDA)** — distributions, scatter plots, correlation heatmap
4. **Feature Engineering** — created new features including:
   - `House_Age` — age of the property at time of sale
   - `Years_Since_Remod` — time since last renovation
   - `Total_SF` — combined basement + above-ground area
   - `Has_Garage`, `Has_Fireplace`, `Has_CentralAir` — binary flags
5. **Model Building** — trained and compared 5 regression models
6. **Evaluation** — assessed models using MAE, RMSE, and R²
7. **Feature Importance** — identified the most influential predictors

---

## 🤖 Models Compared

| Model | Notes |
|-------|-------|
| Linear Regression | Baseline model |
| Ridge Regression | L2 regularisation |
| Lasso Regression | L1 regularisation, feature selection |
| Random Forest | Ensemble, handles non-linearity |
| Gradient Boosting | Best overall performance |

---

## 📊 Key Findings

- **Overall Quality** is the single strongest predictor of sale price
- **Total Square Footage** (basement + above ground) is the second most important feature
- **House Age** negatively impacts price — newer homes command a premium
- **Gradient Boosting** and **Random Forest** significantly outperformed linear models
- Feature engineering (especially `Total_SF` and `House_Age`) meaningfully improved model accuracy

---

## ▶️ How to Run

1. Clone this repository or download the files
2. Make sure `House_Price_Prediction.ipynb` and `ames_housing.csv` are in the **same folder**
3. Open the notebook in Jupyter (Anaconda recommended)
4. Run all cells from top to bottom

**Dependencies:**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 👤 Author

**Arman Arabkhani**  
Third-year Computer Science (Data Science) student @ Auckland University of Technology  
📧 armanarabkhani.nz@yahoo.com  
🔗 [LinkedIn](https://www.linkedin.com/in/arman-arabkhani-95903a384/) | [GitHub](https://github.com/AremonNZ)
