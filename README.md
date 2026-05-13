# 🧠 Data Science Projects

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-green?style=flat&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

---

## 📌 About

A collection of **5 end-to-end Data Science projects** built with Python, each tackling a real-world problem using publicly available datasets. The projects cover the full data science pipeline — data loading, cleaning, exploratory analysis, visualization, model building, and performance evaluation.

Problem domains include **banking**, **healthcare**, **insurance**, and **customer analytics**, applying techniques across data visualization, binary classification, and regression.

---

## 📂 Repository Structure

```
📦 Data-Science-Projects
 ┣ 📓 Task1_Iris_Visualization.ipynb
 ┣ 📓 Task2_Credit_Risk_Prediction.ipynb
 ┣ 📓 Task3_Customer_Churn_Prediction.ipynb
 ┣ 📓 Task4_Insurance_Claim_Prediction.ipynb
 ┣ 📓 Task5_Personal_Loan_Acceptance.ipynb
 ┗ 📄 README.md
```

---

## 🗂️ Projects Overview

| # | Project | Type | Dataset | Libraries |
|---|---------|------|---------|-----------|
| 1 | Iris Dataset Exploration & Visualization | EDA & Visualization | Iris (seaborn built-in) | pandas, matplotlib, seaborn |
| 2 | Credit Risk Prediction | Binary Classification | Loan Prediction (Kaggle) | scikit-learn, pandas, seaborn |
| 3 | Customer Churn Prediction | Binary Classification | Churn Modelling (Kaggle) | scikit-learn, pandas, seaborn |
| 4 | Insurance Claim Amount Prediction | Regression | Medical Cost Personal (Kaggle) | scikit-learn, pandas, seaborn |
| 5 | Personal Loan Acceptance Prediction | Binary Classification | Bank Loan Modelling (Kaggle) | scikit-learn, pandas, seaborn |

---

## 📓 Project Details

---

### 📊 Project 1 — Exploring and Visualizing the Iris Dataset

**Objective:** Load, inspect, and visualize a structured dataset to uncover patterns and relationships between features using core Python visualization libraries.

**Dataset:** Iris Dataset — built directly into seaborn, no download required.

**Approach:**
- Loaded and inspected the dataset using `.shape`, `.columns`, and `.head()`
- Reviewed statistical summaries and checked for missing values
- Built scatter plots, histograms, box plots, a pair plot, and a correlation heatmap

**Key Insights:**
- Iris Setosa is fully separable from the other two species on petal dimensions alone
- Petal length and petal width have a correlation of **0.96** — they carry nearly identical information
- Sepal width is the weakest feature for distinguishing species
- The dataset is perfectly balanced with 50 samples per species and no missing values

---

### 🏦 Project 2 — Credit Risk Prediction

**Objective:** Predict whether a loan applicant is likely to default, helping financial institutions make faster and safer lending decisions.

**Dataset:** [Loan Prediction Dataset — Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)

**Approach:**
- Handled missing values using mode imputation for categorical columns and median for numerical
- Visualized loan amounts, applicant income, education level, and credit history
- Trained **Logistic Regression** and **Decision Tree** classifiers
- Evaluated with accuracy score, confusion matrix, and classification report

**Key Insights:**
- Credit history is the single most powerful predictor of loan approval
- Higher income alone does not guarantee approval without a good credit history
- Logistic Regression achieved **~80–82% accuracy** and is preferred for interpretability
- The model can automate initial loan screening and significantly reduce manual processing time

---

### 📉 Project 3 — Customer Churn Prediction (Bank Customers)

**Objective:** Identify which bank customers are at risk of leaving so the bank can take proactive retention action before losing them.

**Dataset:** [Churn Modelling Dataset — Kaggle](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling)

**Approach:**
- Dropped non-predictive identifier columns (RowNumber, CustomerId, Surname)
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

### 🏥 Project 4 — Predicting Insurance Claim Amounts

**Objective:** Estimate medical insurance charges based on personal attributes such as age, BMI, and smoking status to help insurers set accurate and fair premiums.

**Dataset:** [Medical Cost Personal Dataset — Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) *(also auto-downloads via public GitHub mirror — no Kaggle account needed)*

**Approach:**
- Label encoded sex and smoker; One-Hot encoded region
- Visualized the impact of BMI, age, and smoking status on charges
- Trained **Linear Regression** as a baseline and **Random Forest Regressor** for non-linear patterns
- Evaluated using **MAE**, **RMSE**, and **R²**
- Plotted actual vs predicted values and a residual plot

**Key Insights:**
- Smoking is the most powerful predictor — smokers pay **3–4× more** than non-smokers with identical profiles
- Obese smokers (BMI > 30) form the highest-cost segment by a significant margin
- Random Forest significantly outperformed Linear Regression (**R² ~0.87 vs ~0.75**)
- Region has minimal impact — insurance pricing is fairly uniform across US regions

---

### 🎯 Project 5 — Personal Loan Acceptance Prediction

**Objective:** Predict which bank customers are most likely to accept a personal loan offer, enabling targeted and cost-efficient marketing campaigns.

**Dataset:** [Bank Loan Modelling Dataset — Kaggle](https://www.kaggle.com/datasets/itsmesunil/bank-loan-modelling) *(notebook includes a synthetic fallback dataset if the URL is unavailable)*

**Approach:**
- Cleaned data — removed invalid entries and dropped the ID column
- Explored income, age, education, family size, credit card spend, and CD account holdings
- Trained **Logistic Regression**, **Decision Tree**, and **Random Forest** classifiers
- Evaluated with accuracy, confusion matrix, classification report, and **ROC-AUC curve**
- Segmented customers by income group to identify the highest-value target profile

**Key Insights:**
- Income is the #1 predictor — customers earning above $100k accept at a far higher rate
- CD Account holders are the most valuable target segment for loan campaigns
- Graduate and postgraduate customers accept significantly more than undergraduates
- Random Forest achieved **~95–96% accuracy** and an **AUC of ~0.98**
- Using this model, a bank could reduce marketing spend by ~75–80% while maintaining conversion quality

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

### Option 1 — Google Colab (Recommended — no setup needed)
1. Open [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Open Notebook → GitHub**
3. Paste this repository URL and select any notebook
4. Click **Runtime → Run All**
5. Most datasets auto-download inside the first few cells

### Option 2 — Run Locally
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/Data-Science-Projects.git
cd Data-Science-Projects

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch Jupyter
jupyter notebook
```

---

## 📥 Dataset Sources

| Project | Dataset | Source |
|---------|---------|--------|
| Project 1 | Iris Dataset | Built into seaborn — `sns.load_dataset('iris')` |
| Project 2 | Loan Prediction Dataset | [Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset) |
| Project 3 | Churn Modelling Dataset | [Kaggle](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling) |
| Project 4 | Medical Cost Personal Dataset | [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) / Auto-download |
| Project 5 | Bank Loan Modelling Dataset | [Kaggle](https://www.kaggle.com/datasets/itsmesunil/bank-loan-modelling) / Synthetic fallback |

> **Note:** Projects 1 and 4 do not require a Kaggle account. Projects 2, 3, and 5 include auto-download cells that work without logging in. If they fail, download the CSV from the Kaggle link and upload it to Colab using the manual upload cell provided inside each notebook.

---

## 📊 Results Summary

| Project | Best Model | Best Metric |
|---------|-----------|-------------|
| Project 1 | No model — EDA only | Visual insights across 3 species |
| Project 2 | Logistic Regression | Accuracy ~80–82% |
| Project 3 | Random Forest | Accuracy ~86–87% |
| Project 4 | Random Forest Regressor | R² ~0.87, MAE ~$2,500 |
| Project 5 | Random Forest | Accuracy ~95–96%, AUC ~0.98 |
