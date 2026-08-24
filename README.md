# 🏠 House Price Prediction using Machine Learning

## 📌 Overview

This project is an end-to-end **Machine Learning Regression** project that predicts residential house prices using a real-world **Kaggle House Prices** dataset. It demonstrates the complete machine learning workflow including data cleaning, exploratory data analysis (EDA), feature engineering, model training, evaluation, and final model selection.

The project was developed as part of an internship assignment for **Business Analytics**.

---

## 🎯 Objective

Build a machine learning model that predicts house prices while demonstrating:

- Data preprocessing
- Exploratory Data Analysis
- Feature engineering
- Regression model building
- Model evaluation
- Comparison of multiple machine learning algorithms

---

## 📂 Dataset

- **Source:** Kaggle House Prices Dataset
- **Target Variable:** `price`

### Features Used

- Bedrooms
- Bathrooms
- Living Area (`sqft_living`)
- Lot Size (`sqft_lot`)
- Floors
- Waterfront
- View
- Condition
- Above Ground Area
- Basement Area
- Year Built
- Year Renovated
- City
- State ZIP

### Removed Features

- `date`
- `street`
- `country`

These columns were excluded because they were either non-informative or unsuitable for prediction.

---

## 🔄 Project Workflow

```text
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Feature Engineering
   │
   ▼
Train-Test Split (80:20)
   │
   ▼
Model Training
   │
   ▼
Model Evaluation
   │
   ▼
Best Model Selection
```

---

## 🧹 Data Preprocessing

The dataset was prepared through several preprocessing steps:

- Inspected dataset structure
- Checked missing values
- Removed duplicate records
- Removed invalid house prices (zero or negative values)
- Converted categorical variables using **One-Hot Encoding**
- Applied preprocessing with **ColumnTransformer**
- Split data into **80% training** and **20% testing** using `random_state=42`

---

## 📊 Exploratory Data Analysis

Six meaningful visualizations were created to understand relationships between house prices and property features.

### Visualizations

1. House Price Distribution
2. House Price vs Living Area
3. Correlation Heatmap
4. House Price vs Bedrooms
5. House Price vs Bathrooms
6. House Price by Waterfront

These visualizations helped identify important patterns before model development.

---

## 🤖 Machine Learning Models

Three regression models were trained using the same training and testing framework.

| Model | Purpose |
|--------|---------|
| Linear Regression | Baseline regression model |
| Decision Tree Regressor | Captures nonlinear relationships |
| Random Forest Regressor | Ensemble learning model |

---

## 📈 Model Evaluation

The models were evaluated using four regression metrics.

- **MAE** – Mean Absolute Error
- **MSE** – Mean Squared Error
- **RMSE** – Root Mean Squared Error
- **R² Score** – Coefficient of Determination

### Performance Results

| Model | MAE | RMSE | R² Score |
|--------|------------|------------|----------|
| **Linear Regression** | 139,638.89 | **232,409.25** | **0.6369** |
| Decision Tree | 149,182.95 | 300,352.01 | 0.3936 |
| Random Forest | **121,307.27** | 319,894.63 | 0.3121 |

### Final Model

Although **Random Forest** achieved the lowest Mean Absolute Error, **Linear Regression** was selected as the final model because it achieved:

- Highest R² Score
- Lowest RMSE
- Lowest MSE
- Strongest overall performance across multiple evaluation metrics

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📁 Project Structure

```text
House_Price_Prediction/
│
├── data/
│   └── House_Price.csv
│
├── notebook/
│   └── House_price_Prediction.ipynb
│
├── report/
│   └── House_price_prediction_report.pdf
│
├── presentation/
│   └── House_Price_Prediction_Presentation.pptx
│
├── outputs/
│   ├── charts/
│   └── predictions.csv
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/House-Price-Prediction.git
cd House-Price-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
python -m notebook
```

Open:

```text
House_price_Prediction.ipynb
```

---

## 🏡 Sample Prediction

| Feature | Value |
|----------|-------|
| Bedrooms | 3 |
| Bathrooms | 2 |
| Living Area | 1500 sqft |
| Lot Size | 5000 sqft |
| Floors | 1 |
| Year Built | 1995 |

**Predicted Price:** Generated using the trained Linear Regression model.

---

## 📌 Future Improvements

- Hyperparameter tuning
- XGBoost implementation
- LightGBM comparison
- Streamlit web application
- Cloud deployment
- Interactive dashboard

---

## 🎓 Learning Outcomes

This project demonstrates practical experience in:

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Regression Modeling
- Model Evaluation
- Scikit-learn Pipelines
- Machine Learning Workflow
- Professional Documentation

---

## 📦 Deliverables

The project includes:

- Jupyter Notebook (`.ipynb`)
- Kaggle Dataset
- Project Report (3–5 pages)
- Presentation (8–10 slides)
- Well-commented source code

---

## 👨‍💻 Author

**Himanshu Tomar**

**Business Analytics | Machine Learning Internship Project**

Developed using **Python, Jupyter Notebook, Pandas, Matplotlib, and Scikit-learn**.
