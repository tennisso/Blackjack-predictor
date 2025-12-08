# 🃏KAGGLE - BLACKJACK OUTCOME ANALYSIS (IDS2025 project)
### *Analyzing and predicting Blackjack results using data science*

**Team members:**
- Markkus Pokrovski
- Hugo Tristan Tammik
- Thomas Tennisson

## 📘 Project Overview

This projext explores how **data science and machine learning** can be applied to analyze and predict outcomes in the game of **Blackjack**. Using a real-world Kaggle dataset (61.77 MB) containing **900,000 recorded Blackjack hands** with details about player and dealer cards, bets, and results, we investigate which features influence win/loss outcomes and evaluate multiple prediction models. <br>(Link to the dataset: https://www.kaggle.com/datasets/mojocolors/900000-hands-of-blackjack-results )

## 🎯 Motivation

Our motivation is to explore how data-driven methods can reveal meaningful patterns in blackjack outcomes. By analyzing a large real-world dataset, we aim to apply and strengthen the data-mining skills learned in the IDS2025 course.

## 🎯 Project Goals

### **Goal 1 — Discover frequent patterns**  
Identify patterns such as:
- Which starting totals lead to the highest win rates?
- How do soft hands compare to hard hands?
- How do player totals interact with dealer upcards?

### **Goal 2 — Build predictive models**  
Train several ML models to predict *win vs. loss*:
- Decision Tree  
- k-Nearest Neighbours  
- Random Forest  
- LightGBM  
- Logistic Regression  

### **Goal 3 — Evaluate performance**  
Compare models by:
- Accuracy  
- Confusion matrix  
- ROC curve & AUC  
- Feature importance

## 📂 Repository Structure

```markdown
Blackjack-predictor/
├── 📁 .ipynb_checkpoints    # Folder for notebook checkpoints
├── 📄 E4_report.pdf         # Project report
├── 📄 Kood.ipynb            # Our initial Python notebook.
├── 📄 KoodV2.ipynb          # Python notebook, which contains the final version of our code.      
├── 📄 README.md             # Information about the project         
└── 📁 data.zip              # Our dataset
```

## 🔁 How to Replicate Our Analysis
You can fully reproduce our work using the steps below.
### **1. Clone this repository**
```bash
git clone https://github.com/tennisso/Blackjack-predictor.git
cd Blackjack-predictor
```

### **2. Extract the data.zip into the folder**
### **3. Run the notebook**
```bash
jupyter notebook
```

## 🔍 What Our Code Does
### ▶️ **Step 1 - Data Loading**
Remove useless columns, inspect types, check missing values.

### ▶️ **Step 2 - Exploratory Data Analysis (EDA)**
Plots and calculations for:
- player starting totals
- dealer upcard
- soft vs. non-soft hands
- win-rate heatmaps
- correlations

### ▶️ **Step 3 - Feature Engineering**
Includes strategic blackjack features such as:
- soft-hand indicator
- pair indicator
- dealer strength category
- player risk zone
- advantage metric

### ▶️ **Step 4 - Machine Learning Models**
Models built:
- Logistic Regression
- Decision Tree
- Random Forest
- k-Nearest Neighbours
- LightGBM
- Hyperparameter tuning using RandomizedSearcgCV

### ▶️ **Step 5 - Evaluation**
We evaluate using:
- Accuracy
- Confusion Matrix
- ROC-AUC
- Feature Importance Ranking

## 📊 Key Findings
- The player's starting total and dealer's upcard are the strongest predictors of outcome.
- Engineered features (dealer strength, advantage metric) improveed all models.
- Random Forest and LightGBM achieved the highest accuracy.
