# HR Analytics — Predict Employee Attrition

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-yellow?logo=powerbi)
![Sklearn](https://img.shields.io/badge/Sklearn-ML-orange?logo=scikit-learn)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> Internship Project | Elevate Labs | Data Analyst Domain

---

## 📌 Objective

Analyze HR data to understand the main causes of employee resignation and build a machine learning model to predict future attrition — helping organizations take proactive retention actions.

---

## 📂 Dataset

- **Source:** [IBM HR Analytics Employee Attrition Dataset — Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Rows:** 1,470 employees
- **Features:** 35 columns
- **Target:** `Attrition` (Yes / No)
- **Missing Values:** None

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Google Colab) | Data analysis & ML model building |
| Pandas & NumPy | Data manipulation |
| Matplotlib & Seaborn | Data visualization |
| Scikit-learn | Logistic Regression, Decision Tree, Metrics |
| SHAP | Model explainability |
| Power BI Desktop | Interactive dashboard |

---

## 📊 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Attrition distribution — 16.12% overall attrition rate
- Department-wise attrition analysis
- Age group vs attrition
- Monthly income vs attrition
- Overtime impact on attrition
- Job satisfaction vs attrition
- Correlation heatmap of all features

### 2. Data Preprocessing
- Dropped irrelevant columns: `EmployeeCount`, `EmployeeNumber`, `Over18`, `StandardHours`
- Label encoded all categorical variables
- Handled class imbalance using **oversampling** (1,233 No → balanced with 237 Yes)

### 3. ML Model Building

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 69.23% |
| Decision Tree | **81.58%** ✅ |

- Confusion matrix plotted for both models
- Decision Tree selected as the best model

### 4. SHAP Analysis
- Applied `TreeExplainer` on the Decision Tree model
- Identified top 10 features driving attrition
- Visualized as SHAP bar summary plot

### 5. Power BI Dashboard
- 6 interactive visuals
- 3 slicers: Department, Gender, MaritalStatus
- Consistent Red (Attrition=Yes) / Green (Attrition=No) color theme

---

## 📈 Key Findings

- Employees working **overtime** have 30%+ attrition rate
- **26-35 age group** has the highest attritions
- Employees who left earned avg **$4,787/month** vs **$6,833** for those who stayed
- **Sales department** has the highest attrition rate
- Low job satisfaction (Level 1) correlates with higher attrition

---

## 🗂️ Repository Structure

```
HR-Attrition-Analysis/
│
├── dataset/
│   └── HR-Employee-Attrition.csv
│
├── notebook/
│   └── HR_Analytics_Predict_Employee_Attrition.ipynb
│
├── dashboard/
│   └── HR_Attrition_Dashboard.pbix
│
├── report/
│   └── HR_Attrition_Project_Report.pdf
│   └──HR_Attrition_Prevention_Suggestions.pdf 
|
└── README.md
```

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/jayanthb2005/HR-Attrition-Analysis.git
```

2. Open `notebook/HR_Analytics_Predict_Employee_Attrition.ipynb` in Google Colab

3. Upload `HR-Employee-Attrition.csv` when prompted

4. Run all cells sequentially

---

## 📋 Deliverables

- ✅ Python Notebook (EDA + ML + SHAP)
- ✅ Power BI Dashboard
- ✅ Project Report (PDF)

---

## 💡 Attrition Prevention Suggestions

- Reduce overtime and introduce flexible work arrangements
- Conduct regular salary reviews for employees aged 26-35
- Introduce career growth programs and timely promotions
- Closely monitor Sales department employees
- Implement quarterly employee satisfaction surveys

---

## 👤 Author

**Vinay N V**

Data Analyst Intern — Elevate Labs
