AI-Projects

A curated portfolio of my AI and machine learning work.
This repository serves as an index. Each section below links to a separate project repository with full code, data, and documentation.

📂 Project List
Project	Description	Tech Stack	Link
🧬 Breast Cancer Malignancy Predictor	Classifies tumors as malignant or benign using diagnostic features from the Wisconsin dataset.	Python, scikit-learn, pandas, seaborn, matplotlib	View Repo

🌲 Forest Fire Predictor	Predicts severity of forest fires using regression models, Keras neural networks, and 7-day historical weather data from an API.	Python, scikit-learn, Keras, TensorFlow, API Integration	View Repo

🧠 Multi Agent Financial Analysis System	Autonomous agent workflow that researches public financial info, synthesizes insights, and produces auditable briefs with citations.	CrewAI, Python, OpenAI GPT-4o, Claude 3.5 Sonnet	View Repo
🧠 Multi Agent Financial Analysis System

Autonomous research system that coordinates multiple agents to collect financial data, reason over it, and generate stakeholder-ready briefs with sources.
Developed by AAI-520-02 Final Project Group 4 at the University of San Diego.

📊 Project Overview

• Capabilities: multi-agent planning, evidence capture, consistency checks, report generation
• Models: GPT-4o and Claude 3.5 Sonnet orchestrated through CrewAI
• Outputs: structured JSON source captures plus a readable PDF or Markdown brief

🧰 Tools

• CrewAI for agent orchestration
• Python for glue code and evaluation scripts

▶️ How to Run

Create and activate a virtual environment

Install dependencies from requirements.txt

Set environment variables OPENAI_API_KEY and ANTHROPIC_API_KEY

Run a sample task

 python -m src.run --task "Analyze the latest earnings of a Fortune 100 company and summarize risks and opportunities"


Review generated artifacts in outputs and reports

🤝 Team and my focus

• Team: AAI-520-02 Final Project Group 4
• Thomas Geraci focus: project structure and documentation quality, reliability fixes around data adapters and artifact saving, evaluation mindset carried over from prior Linear Regression and Keras work

🧬 Breast Cancer Malignancy Predictor

A supervised machine learning project to predict breast cancer malignancy using diagnostic features from the Wisconsin Breast Cancer Dataset.
Developed as part of the AAI-500 Capstone Project. M.S. Applied Artificial Intelligence University of San Diego.

📊 Project Overview

• Dataset: Wisconsin Diagnostic Breast Cancer
• Techniques: data cleaning, EDA, feature selection, classification modeling
• Models: logistic regression, random forest classifier
• Evaluation: confusion matrix, ROC curve, F1-score, precision, recall
• Tools: Python, pandas, scikit-learn, seaborn, matplotlib

🛠️ Workflow
1️⃣ Data Cleaning and Preprocessing

• Dropped unnecessary columns id and unnamed indices
• Encoded target diagnosis as 1 for malignant and 0 for benign
• Verified no missing values

2️⃣ Exploratory Data Analysis

• Histograms, boxplots, heatmaps, pairplots
• Correlations and top feature selection

3️⃣ Model Building and Evaluation

• Trained logistic regression and random forest
• Evaluated with confusion matrices, ROC curves, and classification reports

👥 Team Members and Roles
Team Member	Role	Responsibilities
Denis Mulabegovic	Model Builder	t-tests for key features, built LR and RF models, model selection docs, modeling support
Thomas Geraci	Data Engineer and Analyst	data cleaning and preprocessing, EDA, visualizations, authored data prep and EDA sections
Pros Loung	Model Evaluator and Report Lead	evaluations, metrics, final report, conclusion section
🌲 Forest Fire Predictor

A machine learning project predicting forest fire severity using weather data and multiple regression-based models.
View Full Repository

Developed as part of the AAI-501 course M.S. Applied Artificial Intelligence University of San Diego.

📊 Project Overview

• Dataset: UCI Forest Fire plus integrated real-time weather API
• Techniques: data cleaning, feature engineering, scaling, model comparison
• Models: Linear Regression, Random Forest, Lasso Regression, Keras neural network
• Evaluation: R² and MAE
• Tools: Python, pandas, scikit-learn, matplotlib, seaborn, Keras, API integration

🛠️ Workflow
1️⃣ Data Preparation

• Removed irrelevant features and handled missing values
• Scaled numerical data
• Integrated 7-day weather API

2️⃣ Model Development

• Linear Regression for baseline interpretability
• Random Forest for complex interactions
• Lasso for feature selection and regularization
• Keras model for nonlinear patterns

3️⃣ Model Evaluation

• Compared R² and MAE across models
• Residual and prediction vs actual plots
• Feature importance from tree-based models

👥 Team Members and Roles
Team Member	Role	Responsibilities
Thomas Geraci	Data Engineer and Analyst	data cleaning, transformation, scaling, Linear Regression, residual and prediction plots, contributions to Keras and weather API sections
Daniel Sims	Random Forest Specialist	implementation and tuning, feature importance plots, summary stats
Arslan Isaac	Lasso Regression Specialist	Lasso implementation, feature selection analysis, documentation support
All Members	Collaborative Work	integrated 7-day weather API and Keras model
