# AI-Projects
# 🧬 Breast Cancer Malignancy Predictor

A supervised machine learning project to predict breast cancer malignancy using diagnostic features from the Wisconsin Breast Cancer Dataset.  
Developed as part of the AAI-500 Capstone Project — *M.S. Applied Artificial Intelligence* — University of San Diego.

---

## 📊 Project Overview

- **Dataset:** Wisconsin Diagnostic Breast Cancer (WDBC)
- **Techniques Used:** Data Cleaning, Exploratory Data Analysis (EDA), Feature Selection, Classification Modeling
- **Models Built:** Logistic Regression, Random Forest Classifier
- **Evaluation Metrics:** Confusion Matrix, ROC Curve, F1-score, Precision, Recall
- **Tools:** Python, pandas, scikit-learn, seaborn, matplotlib

---

## 🛠️ Workflow

### 1️⃣ Data Cleaning & Preprocessing
- Dropped unnecessary columns (`id`, unnamed index columns).
- Encoded categorical target variable `diagnosis`:
  - Malignant → `1`
  - Benign → `0`
- Verified no missing or null values remained.

### 2️⃣ Exploratory Data Analysis (EDA)
- Created histograms, boxplots, heatmaps, and pairplots.
- Analyzed feature distributions and correlations.
- Selected top features most correlated with cancer diagnosis.

### 3️⃣ Model Building & Evaluation
- Trained logistic regression and random forest classifiers.
- Evaluated models using:
  - Confusion Matrices
  - ROC Curves
  - Classification Reports (Precision, Recall, F1-Score)

---

## 👥 Team Members & Roles

| Team Member | Role | Responsibilities |
| ------------ | ---- | ----------------- |
| **Denis Mulabegovic (Team Leader)** | Model Builder | - Conducted t-tests for key features<br>- Built logistic regression and random forest models<br>- Contributed to model selection documentation<br>- Provided modeling support |
| **Thomas Geraci** | Data Engineer & Analyst | - Handled data cleaning and preprocessing<br>- Performed exploratory data analysis (EDA)<br>- Created visualizations (heatmaps, boxplots, pairplots)<br>- Authored data prep and EDA sections |
| **Pros Loung** | Model Evaluator & Report Lead | - Evaluated models using confusion matrices and ROC curves<br>- Calculated classification metrics (e.g. F1-score)<br>- Compiled and formatted final report<br>- Wrote evaluation and conclusion sections |

---

## 📂 Repository Structure
Breast-Cancer-Predictor
├── Breast_Cancer_Predictor_Project.ipynb   
├── data.csv                               
└── README.md                           
