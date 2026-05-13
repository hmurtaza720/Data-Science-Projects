# 🧠 DevelopersHub Data Science & Analytics Internship

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-green?style=flat&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

> **Internship:** Data Science & Analytics  
> **Company:** DevelopersHub Corporation  
> **Duration:** May 2026  
> **Notebooks:** Google Colab (.ipynb)  
> **Tasks Completed:** 5 out of 5 ✅

---

## 📌 About This Repository

This repository contains all **5 completed project tasks** from my Data Science & Analytics Internship at **DevelopersHub Corporation**. Each task is a fully self-contained Jupyter Notebook covering the complete data science pipeline — from raw data loading and cleaning, through exploratory analysis and visualization, to machine learning model building and evaluation.

The projects span core data science problem types including **data visualization**, **binary classification**, **regression**, and **customer segmentation**, using real-world datasets from Kaggle and other public sources.

---

## 📂 Repository Structure

```
📦 DevelopersHub-Data-Science-Internship
 ┣ 📓 Task1_Iris_Visualization.ipynb
 ┣ 📓 Task2_Credit_Risk_Prediction.ipynb
 ┣ 📓 Task3_Customer_Churn_Prediction.ipynb
 ┣ 📓 Task4_Insurance_Claim_Prediction.ipynb
 ┣ 📓 Task5_Personal_Loan_Acceptance.ipynb
 ┗ 📄 README.md
```

---

## 🗂️ Task Overview

| # | Task | Type | Dataset | Libraries |
|---|------|------|---------|-----------|
| 1 | Iris Dataset Exploration & Visualization | EDA & Visualization | Iris (seaborn built-in) | pandas, matplotlib, seaborn |
| 2 | Credit Risk Prediction | Binary Classification | Loan Prediction (Kaggle) | scikit-learn, pandas, seaborn |
| 3 | Customer Churn Prediction | Binary Classification | Churn Modelling (Kaggle) | scikit-learn, pandas, seaborn |
| 4 | Insurance Claim Amount Prediction | Regression | Medical Cost Personal (Kaggle) | scikit-learn, pandas, seaborn |
| 5 | Personal Loan Acceptance Prediction | Binary Classification | Bank Loan Modelling (Kaggle) | scikit-learn, pandas, seaborn |

---

## 📓 Task Details

---

### ✅ Task 1 — Exploring and Visualizing the Iris Dataset

**Objective:** Understand how to load, inspect, and visualize a structured dataset using core Python libraries — with no machine learning model involved.

**Dataset:** Iris Dataset — built directly into seaborn, no download required.

**Approach:**
- Loaded and inspected the dataset using `.shape`, `.columns`, and `.head()`
- Checked for missing values and reviewed statistical summaries
- Built scatter plots, histograms, box plots, a pair plot, and a correlation heatmap

**Key Insights:**
- Iris Setosa is fully separable from the other two species on petal dimensions alone
- Petal length and petal width have a correlation of **0.96** — they carry nearly identical information
- Sepal width is the weakest feature for species classification
- The dataset is perfectly balanced with no missing values

---

### ✅ Task 2 — Credit Risk Prediction

**Objective:** Predict whether a loan applicant is likely to default, helping banks make faster and safer lending decisions.

**Dataset:** [Loan Prediction Dataset — Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)

**Approach:**
- Handled missing values using mode imputation for categorical columns and median for numerical
- Visualized loan amounts, applicant income, education level, and credit history
- Trained **Logistic Regression** and **Decision Tree** classifiers
- Evaluated with accuracy score, confusion matrix, and classification report

**Key Insights:**
- Credit history is the single most powerful predictor of loan approval
- Higher income alone does not guarantee approval without good credit history
- Logistic Regression achieved **~80–82% accuracy** and is preferred for interpretability
- The model can automate initial screening and significantly reduce processing time

---

### ✅ Task 3 — Customer Churn Prediction (Bank Customers)

**Objective:** Identify which bank customers are at risk of leaving so the bank can take proactive retention action.

**Dataset:** [Churn Modelling Dataset — Kaggle](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling)

**Approach:**
- Dropped non-predictive identifiers (RowNumber, CustomerId, Surname)
- Applied Label Encoding to Gender and One-Hot Encoding to Geography
- Built visualizations for age, balance, number of products, salary, and credit score
- Trained **Random Forest** and **Gradient Boosting** classifiers
- Analysed feature importance to identify the top churn drivers

**Key Insights:**
- Age is the #1 churn driver — customers aged 40–60 are at the highest risk
- Germany has nearly double the churn rate of France and Spain
- Customers with only 1 product are far more likely to leave than those with 2
- Both models achieved **~86–87% accuracy**

---

### ✅ Task 4 — Predicting Insurance Claim Amounts

**Objective:** Estimate how much a customer will be charged for medical insurance based on personal attributes, helping insurers set fair and accurate premiums.

**Dataset:** [Medical Cost Personal Dataset — Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) *(also available via public GitHub mirror — auto-downloads in notebook)*

**Approach:**
- Label encoded sex and smoker; One-Hot encoded region
- Visualized the impact of BMI, age, and smoking status on charges using scatter plots, box plots, and violin plots
- Trained **Linear Regression** (baseline) and **Random Forest Regressor**
- Evaluated using **MAE**, **RMSE**, and **R²**
- Plotted actual vs predicted values and residual plots

**Key Insights:**
- Smoking is the most powerful predictor — smokers pay **3–4× more** than non-smokers
- Obese smokers (BMI > 30) represent the highest-cost segment by a large margin
- Random Forest significantly outperformed Linear Regression (**R² ~0.87 vs ~0.75**)
- Region has minimal impact on charges — pricing is fairly uniform across US regions

---

### ✅ Task 5 — Personal Loan Acceptance Prediction

**Objective:** Predict which customers are most likely to accept a personal loan offer, enabling targeted and cost-efficient marketing campaigns.

**Dataset:** [Bank Loan Modelling Dataset — Kaggle](https://www.kaggle.com/datasets/itsmesunil/bank-loan-modelling) *(notebook also includes a synthetic fallback dataset if the URL is unavailable)*

**Approach:**
- Cleaned data — removed invalid entries, dropped the ID column
- Explored income, age, education, family size, credit card spend, and CD account
- Trained **Logistic Regression**, **Decision Tree**, and **Random Forest** classifiers
- Evaluated with accuracy, confusion matrix, classification report, and **ROC-AUC curve**
- Segmented customers by income group and identified the ideal target profile

**Key Insights:**
- Income is the #1 predictor — customers earning above $100k accept at a far higher rate
- CD Account holders are the most valuable marketing target segment
- Graduate and postgraduate customers accept significantly more than undergraduates
- Random Forest achieved **~95–96% accuracy** and an **AUC of ~0.98**
- Using this model, a bank can reduce marketing spend by ~75–80% while maintaining conversion quality

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python 3.10** | Core programming language |
| **Pandas** | Data loading, cleaning, and manipulation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Base plotting and chart creation |
| **Seaborn** | Statistical visualizations |
| **Scikit-learn** | ML models, preprocessing, and evaluation metrics |
| **Google Colab** | Cloud-based Jupyter Notebook environment |

---

## 🚀 How to Run Any Notebook

### Option 1 — Google Colab (Recommended, no setup required)
1. Open [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Open Notebook → GitHub**
3. Paste this repository URL and select any notebook
4. Click **Runtime → Run All**
5. Most datasets auto-download inside the first few cells

### Option 2 — Run Locally
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/DevelopersHub-Data-Science-Internship.git
cd DevelopersHub-Data-Science-Internship

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch Jupyter
jupyter notebook
```

---

## 📥 Dataset Sources

| Task | Dataset | Source |
|------|---------|--------|
| Task 1 | Iris Dataset | Built into seaborn — `sns.load_dataset('iris')` |
| Task 2 | Loan Prediction Dataset | [Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset) |
| Task 3 | Churn Modelling Dataset | [Kaggle](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling) |
| Task 4 | Medical Cost Personal Dataset | [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) / Auto-download |
| Task 5 | Bank Loan Modelling Dataset | [Kaggle](https://www.kaggle.com/datasets/itsmesunil/bank-loan-modelling) / Synthetic fallback |

> **Note:** Tasks 1 and 4 do not require a Kaggle account. Tasks 2, 3, and 5 include auto-download cells that work without logging in. If they fail, simply download the CSV from the Kaggle link and upload it to Colab using the manual upload cell provided inside each notebook.

---

## 📊 Results Summary

| Task | Model Used | Best Metric |
|------|-----------|-------------|
| Task 1 | No model — EDA only | Visual insights across 3 species |
| Task 2 | Logistic Regression | Accuracy ~80–82% |
| Task 3 | Random Forest | Accuracy ~86–87% |
| Task 4 | Random Forest Regressor | R² ~0.87, MAE ~$2,500 |
| Task 5 | Random Forest | Accuracy ~95–96%, AUC ~0.98 |

---

## 🙏 Acknowledgements

- **DevelopersHub Corporation** for providing this internship opportunity and structured task list
- **Kaggle** for the publicly available datasets used across tasks 2–5
- **Scikit-learn, Pandas, Seaborn, and Matplotlib** open-source communities
