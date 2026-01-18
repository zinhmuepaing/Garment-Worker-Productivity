# Workers Productivity Classification (AIML Project – Part A)

## 📌 Project Overview
This project focuses on predicting **worker productivity levels** in the garment manufacturing industry using machine learning.  
Productivity is classified into **Low, Medium, and High** based on operational and workforce-related features.

The objective is to understand how production factors influence productivity and to evaluate multiple classification models to identify the most effective approach.

---

## 📊 Dataset
- Source: Garment factory productivity dataset (Bangladesh, 2015)
- Contains daily production records for sewing and finishing teams
- Includes operational, workforce, and efficiency-related variables

**Target variable**
- `productivity` (Low, Medium, High)

---

## 🧹 Data Preparation
Key preprocessing steps:
- Median imputation for skewed variables such as **WIP**
- Cleaning inconsistent categorical values (e.g., department names)
- Context-aware outlier handling
- One-hot encoding for categorical features
- Feature scaling using **MinMaxScaler** for distance- and margin-based models

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was conducted to examine:
- Productivity class distribution
- Productivity differences across departments and quarters
- Relationships between overtime, WIP, and actual productivity
- Correlations among numerical features to identify interactions and multicollinearity

Visualisations include:
- Pie charts
- Stacked bar charts
- Histograms
- Scatter plots
- Correlation heatmaps

---

## 🧠 Models Implemented
The following multi-class classification models were developed and evaluated:

- **Logistic Regression**
- **Support Vector Machine (Linear & RBF)**
- **K-Nearest Neighbours (KNN)**
- **Random Forest**

All models were trained and evaluated using the same data split and metrics to ensure fair comparison.

---

## ⚙️ Feature Engineering
A domain-driven feature was introduced:

- **prod_gap = actual_productivity − targeted_productivity**

This feature captures performance deviation relative to expectations and significantly improves model performance across all classifiers.

---

## 📈 Model Evaluation
Models were evaluated using:
- Accuracy
- Precision, Recall, and F1-score
- Confusion matrices

### Key Findings
- **Random Forest** achieved the best overall performance
- Feature engineering had a greater impact than changing models alone
- Medium productivity was the most challenging class to predict
- Tree-based models handled non-linear interactions most effectively

---

## 🏆 Final Model
**Random Forest** was selected as the final model due to:
- Highest accuracy
- Balanced performance across all classes
- Robust handling of feature interactions without requiring feature scaling

---

## 🤖 GenAI Usage
AI tools were used responsibly for:
- Brainstorming visualisation ideas
- Exploring alternative modelling strategies
- Reviewing feature engineering options

All suggestions were critically evaluated, and final implementations were developed and validated independently.

---

## 📁 Project Structure
