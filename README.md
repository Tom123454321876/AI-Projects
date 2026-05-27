# AI-Projects

A curated portfolio of my artificial intelligence, machine learning, agentic AI, and IoT forecasting work.  
This repository serves as an index for selected academic and applied projects, with links to notebooks, repositories, code, data workflows, and documentation.

---

## 📂 Project List

| Project | Description | Tech Stack | Link |
|---------|-------------|------------|------|
| 🧠 Multi Agent Financial Analysis System | Autonomous agent workflow that researches public financial information, synthesizes insights, and produces auditable briefs with citations. | CrewAI, Python, OpenAI GPT-4o, Claude 3.5 Sonnet, Agentic AI | [View Repo](https://github.com/apadin-repo/AAI-520-02-FINAL-PROJECT-GROUP-4) |
| 🌡️ IoT Sensor Forecasting and Tableau Dashboard | Machine learning IoT project that forecasts building sensor conditions using LSTM and Random Forest models, then exports prediction results for Tableau dashboards. | Python, pandas, NumPy, scikit-learn, TensorFlow/Keras, Matplotlib, Seaborn, Tableau | [View Notebook](./Team_6_Final%20Team%20Project%20Machine%20Learning%20IoT%20Application%20Design%20and%20Implementation.ipynb) |
| 🧬 Breast Cancer Malignancy Predictor | Classifies tumors as malignant or benign using diagnostic features from the Wisconsin dataset. | Python, scikit-learn, pandas, seaborn, matplotlib | [View Repo](https://github.com/Tom123454321876/AI-Projects) |
| 🌲 Forest Fire Predictor | Predicts severity of forest fires using regression models, Keras neural networks, and 7-day historical weather data from an API. | Python, scikit-learn, Keras, TensorFlow, API Integration | [View Repo](https://github.com/Tom123454321876/AAI501-Forest-Fire-Predictor-Final-Project-Group2) |

---

# 🧠 Multi Agent Financial Analysis System

Autonomous research system that coordinates multiple agents to collect financial data, reason over it, and generate stakeholder-ready briefs with sources.  
Developed by AAI-520-02 Final Project Group 4 at the University of San Diego.

### 📊 Project Overview
• Capabilities: multi-agent planning, evidence capture, consistency checks, report generation  
• Models: GPT-4o and Claude 3.5 Sonnet orchestrated through CrewAI  
• Outputs: structured JSON source captures plus a readable PDF or Markdown brief

### 🧰 Tools
• CrewAI for agent orchestration  
• Python for glue code and evaluation scripts

### ▶️ How to Run
1. Create and activate a virtual environment  
2. Install dependencies from requirements.txt  
3. Set environment variables OPENAI_API_KEY and ANTHROPIC_API_KEY  
4. Run a sample task  

```bash
python -m src.run --task "Analyze the latest earnings of a Fortune 100 company and summarize risks and opportunities"
```

5. Review generated artifacts in outputs and reports

### 🤝 Team and my focus
• Team: AAI-520-02 Final Project Group 4  
• Thomas Geraci focus: project structure and documentation quality, reliability fixes around data adapters and artifact saving, evaluation mindset carried over from prior Linear Regression and Keras work

---

# 🌡️ IoT Sensor Forecasting and Tableau Dashboard

A machine learning and IoT analytics project focused on forecasting environmental sensor readings from building data and preparing model outputs for Tableau visualization.  
Developed as part of AAI-530 Data Analytics and Internet of Things at the University of San Diego.

## 📊 Project Overview
• Dataset: IoT building sensor CSV files with timestamped readings  
• Sensors used: Temperature, Humidity, Light, and RSSI  
• Techniques: time-series preprocessing, resampling, missing-value handling, feature engineering, sequence modeling, lag features, and model evaluation  
• Models: LSTM neural network for temperature forecasting and Random Forest Regressor for humidity forecasting  
• Dashboard output: exported `tableau_predictions.csv` containing timestamps, actual values, predicted values, and absolute error fields for Tableau dashboards

## 🛠️ Workflow
### 1️⃣ Data Processing and Preprocessing
• Loaded and cleaned large IoT CSV sensor files  
• Converted Unix timestamps into datetime format  
• Pivoted sensor readings into a wide time-series format  
• Resampled readings into consistent 5-minute intervals  
• Interpolated and filled missing values to prepare the data for modeling

### 2️⃣ Exploratory Data Analysis
• Visualized temperature and humidity trends over time  
• Built a sensor correlation matrix  
• Reviewed autocorrelation, scatter plots, and boxplots to understand sensor behavior  
• Used EDA results to justify time-based modeling decisions

### 3️⃣ LSTM Temperature Forecasting
• Built supervised sliding-window sequences from the IoT time series  
• Used a time-ordered train/validation split to avoid data leakage  
• Scaled features with MinMaxScaler  
• Trained a two-layer LSTM model with dropout and early stopping  
• Evaluated temperature predictions with MAE, RMSE, R², and absolute error plots

### 4️⃣ Random Forest Humidity Forecasting
• Engineered lag features for humidity and temperature  
• Added calendar/time features, including hour, day of week, month, weekend flag, and cyclical encodings  
• Trained a Random Forest Regressor for one-step-ahead humidity forecasting  
• Compared model predictions against a persistence baseline

### 5️⃣ Tableau Export
• Merged temperature and humidity prediction outputs by timestamp  
• Exported a single Tableau-ready CSV with actual values, predictions, and error metrics  
• Structured the output for KPI tiles, time-series charts, and model error visualizations

## 📈 Results
• LSTM Temperature Forecasting: MAE 0.1992, RMSE 0.2449, R² 0.9583  
• Random Forest Humidity Forecasting: MAE 0.1895, RMSE 0.2813, R² 0.9941  
• Exported 220 aligned prediction rows for Tableau visualization

## 👥 Team Members and Roles
| Team Member | Role | Responsibilities |
| ------------ | ---- | ----------------- |
| **Thomas Geraci** | Machine Learning and Forecasting Contributor | LSTM preprocessing, sequence generation, LSTM model design, temperature evaluation, Random Forest preprocessing, humidity forecasting, metrics, and Tableau prediction export |
| **Denis Mulabegovic** | Data Processing and EDA Contributor | CSV loading, timestamp conversion, sensor pivoting, resampling, exploratory analysis, and visual checks |
| **Santosh Kumar** | Data Processing and Project Contributor | Data workflow support, preprocessing design, project validation, and documentation support |

---

# 🧬 Breast Cancer Malignancy Predictor

A supervised machine learning project to predict breast cancer malignancy using diagnostic features from the Wisconsin Breast Cancer Dataset.  
Developed as part of the AAI-500 Capstone Project. *M.S. Applied Artificial Intelligence* University of San Diego.

## 📊 Project Overview
• Dataset: Wisconsin Diagnostic Breast Cancer  
• Techniques: data cleaning, EDA, feature selection, classification modeling  
• Models: logistic regression, random forest classifier  
• Evaluation: confusion matrix, ROC curve, F1-score, precision, recall  
• Tools: Python, pandas, scikit-learn, seaborn, matplotlib

## 🛠️ Workflow
### 1️⃣ Data Cleaning and Preprocessing
• Dropped unnecessary columns `id` and unnamed indices  
• Encoded target `diagnosis` as 1 for malignant and 0 for benign  
• Verified no missing values

### 2️⃣ Exploratory Data Analysis
• Histograms, boxplots, heatmaps, pairplots  
• Correlations and top feature selection

### 3️⃣ Model Building and Evaluation
• Trained logistic regression and random forest  
• Evaluated with confusion matrices, ROC curves, and classification reports

## 👥 Team Members and Roles
| Team Member | Role | Responsibilities |
| ------------ | ---- | ----------------- |
| **Denis Mulabegovic** | Model Builder | t-tests for key features, built LR and RF models, model selection docs, modeling support |
| **Thomas Geraci** | Data Engineer and Analyst | data cleaning and preprocessing, EDA, visualizations, authored data prep and EDA sections |
| **Pros Loung** | Model Evaluator and Report Lead | evaluations, metrics, final report, conclusion section |

---

# 🌲 Forest Fire Predictor

A machine learning project predicting forest fire severity using weather data and multiple regression-based models.  
[View Full Repository](https://github.com/Tom123454321876/AAI501-Forest-Fire-Predictor-Final-Project-Group2)  
Developed as part of the AAI-501 course *M.S. Applied Artificial Intelligence* University of San Diego.

## 📊 Project Overview
• Dataset: UCI Forest Fire plus integrated real-time weather API  
• Techniques: data cleaning, feature engineering, scaling, model comparison  
• Models: Linear Regression, Random Forest, Lasso Regression, Keras neural network  
• Evaluation: R² and MAE  
• Tools: Python, pandas, scikit-learn, matplotlib, seaborn, Keras, API integration

## 🛠️ Workflow
### 1️⃣ Data Preparation
• Removed irrelevant features and handled missing values  
• Scaled numerical data  
• Integrated 7-day weather API

### 2️⃣ Model Development
• Linear Regression for baseline interpretability  
• Random Forest for complex interactions  
• Lasso for feature selection and regularization  
• Keras model for nonlinear patterns

### 3️⃣ Model Evaluation
• Compared R² and MAE across models  
• Residual and prediction vs actual plots  
• Feature importance from tree-based models

## 👥 Team Members and Roles
| Team Member | Role | Responsibilities |
| ------------ | ---- | ----------------- |
| **Thomas Geraci** | Data Engineer and Analyst | data cleaning, transformation, scaling, Linear Regression, residual and prediction plots, contributions to Keras and weather API sections |
| **Daniel Sims** | Random Forest Specialist | implementation and tuning, feature importance plots, summary stats |
| **Arslan Isaac** | Lasso Regression Specialist | Lasso implementation, feature selection analysis, documentation support |
| **All Members** | Collaborative Work | integrated 7-day weather API and Keras model |
