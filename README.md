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

# 🌲 Forest Fire Predictor

A machine learning project predicting forest fire severity using weather data and multiple regression-based models.  
[View Repository](https://github.com/Tom123454321876/AAI501-Forest-Fire-Predictor-Final-Project-Group2)  
Developed as part of the AAI-501 course — *M.S. Applied Artificial Intelligence* — University of San Diego.

---

## 📊 Project Overview

- **Dataset:** UCI Forest Fire Dataset (plus integrated real-time weather API)
- **Techniques Used:** Data Cleaning, Feature Engineering, Scaling, Model Comparison
- **Models Built:** Linear Regression, Random Forest, Lasso Regression, Keras Neural Network
- **Evaluation Metrics:** R² Score, Mean Absolute Error (MAE)
- **Tools:** Python, pandas, scikit-learn, matplotlib, seaborn, Keras, API integration

---

## 🛠️ Workflow

### 1️⃣ Data Preparation
- Removed irrelevant features and handled missing values.
- Scaled numerical data for regression and neural network models.
- Integrated 7-day weather API for short-term prediction enhancement.

### 2️⃣ Model Development
- Implemented Linear Regression for baseline interpretability.
- Applied Random Forest for capturing complex feature interactions.
- Used Lasso Regression for feature selection and regularization.
- Built a Keras deep learning model to detect nonlinear patterns.

### 3️⃣ Model Evaluation
- Compared R² and MAE across models.
- Created residual and prediction vs. actual plots.
- Analyzed feature importance from tree-based models.

---

## 👥 Team Members & Roles

| Team Member | Role | Responsibilities |
| ------------ | ---- | ----------------- |
| **Thomas Geraci** | Data Engineer & Analyst | - Led data cleaning, transformation, and scaling<br>- Implemented Linear Regression<br>- Created residual and predicted vs. actual plots<br>- Contributed to Keras and weather API sections |
| **Daniel** | Random Forest Specialist | - Implemented and tuned Random Forest model<br>- Generated feature importance plots<br>- Summarized statistical results |
| **Arslan** | Lasso Regression Specialist | - Implemented Lasso Regression<br>- Conducted feature selection analysis<br>- Assisted in technical documentation |
| **All Members** | Collaborative Work | - Integrated 7-day weather API<br>- Developed Keras neural network model |

---


## 📂 Repository Structure
Breast-Cancer-Predictor
├── Breast_Cancer_Predictor_Project.ipynb   
├── data.csv                               
└── README.md                           
