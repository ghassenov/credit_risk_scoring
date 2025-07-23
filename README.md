# Credit Risk Scoring Project 🏦📊

## 📌 Project Overview  
This project focuses on building a **machine learning model** to assess **credit risk** by predicting the likelihood of loan default. The workflow includes **data preprocessing**, **exploratory data analysis (EDA)**, and **model training** with tree-based algorithms to achieve optimal predictive performance.  

---

## 📂 Project Structure  

```plaintext
credit_risk_scoring/  
├── 📂 data/  
│   ├── 📂 processed/  
│   │   ├── ✅ df_test.pkl  
│   │   ├── ✅ df_train_full.pkl  
│   │   ├── ✅ df_train.pkl  
│   │   ├── ✅ df_val.pkl  
│   │   ├── ✅ DictVectorizer.pkl  
│   │   ├── ✅ processed_df.pkl  
│   │   ├── ✅ X_train.pkl  
│   │   ├── ✅ X_val.pkl  
│   │   ├── ✅ y_train.pkl  
│   │   └── ✅ y_val.pkl  
│   └── 📂 raw/  
│       └── 📄 CreditScoring.csv  
├── 📂 plots/  
│   ├── 📊 assets_distribution.png  
│   ├── 📊 debt_distribution.png  
│   ├── 📊 income_distribution.png  
│   ├── 📈 Number_of_trees_vs_AUC.png  
│   ├── 📈 Number_of_trees_vs_AUC_depth_tuning.png  
│   └── 📈 Number_of_trees_vs_AUC_min_samples_leaf.png  
├── 📂 src/  
│   ├── 📓 data_preprocessing.ipynb  
│   ├── 📓 EDA.ipynb  
│   └── 📓 model_training.ipynb  
├── 📝 Pipfile  
├── 📝 Pipfile.lock  
└── 📝 README.md

---

## 🔄 Workflow Details

### 1. Data Preprocessing (`data_preprocessing.ipynb`) 🧹
- **Data Loading**: Imported raw `CreditScoring.csv` dataset
- **Standardization**:
  - Uniform column naming conventions
  - Fixed inconsistent value types (numerical → categorical mapping)
- **Data Cleaning**:
  - Corrected misleading missing value encodings
  - Handled outliers and inconsistencies
- **Output**: Prepared clean datasets for EDA and modeling

### 2. Exploratory Data Analysis (`EDA.ipynb`) 🔍
- **Distribution Analysis**:
  - Assets, debt, and income distributions
  - Target variable (`status`) analysis
- **Feature Importance**:
  - Identified key predictors of credit risk
  - Correlation analysis with target variable
- **Visualizations**:
  - Generated distribution plots
  - Created feature importance charts

### 3. Model Training (`model_training.ipynb`) 🤖
- **Algorithm Testing**:
  - 🌳 Decision Trees (baseline)
  - 🌲 Random Forest (improved performance)
  - ⚡ XGBoost (best performer)
- **Model Optimization**:
  - Hyperparameter tuning
  - AUC-based evaluation
  - Feature selection refinement
- **Final Results**:
  - Achieved **83.1% AUC**
  - Generated performance comparison plots

## 🏆 Key Achievements

| Achievement | Impact |
|------------|--------|
| **83.1% AUC Score** | Highly predictive model for credit risk assessment |
| **Comprehensive Data Pipeline** | Reliable, reproducible data processing workflow |
| **Algorithm Comparison** | Evidence-based model selection (XGBoost optimal) |
| **Actionable Insights** | Clear feature importance for business decisions |
| **Production-ready Artifacts** | Serialized models and vectorizers for deployment |

💡 **Business Value**: Enables data-driven lending decisions with reduced risk exposure