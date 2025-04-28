
## Overview
This project aims to **solve customer retention problems** for an e-commerce business by using **Cohort Analysis** and **Predictive Modeling**.  
The goal is to understand customer behavior, identify churn patterns, and proactively predict customers at risk of churning.

The project uses **Cohort Analysis**, **RFM feature engineering**, and **machine learning models** (Random Forest and XGBoost) to predict churn.

---


## 📂 Project Structure

├── **data/**  
│   ├── raw/               # Original datasets  
│   └── processed/         # Cleaned/transformed data  

├── **visualizations/**  
│   ├── cohorts/           # Retention heatmaps  
│   └── eda/               # Exploratory analysis plots  

├── **evaluations/**  
│   ├── confusion_matrices/ # Model performance visuals  
│   └── classification_reports/ # Precision/recall metrics  

├── **models/**            # Saved model files (.pkl or .joblib)  

├── **notebooks/**  
│   ├── 1_eda_cohorts.ipynb  
│   ├── 2_feature_engineering.ipynb  
│   └── 3_model_training.ipynb  

└── **README.md**          # Project documentation  


## Steps Followed

1. **Data Loading**  
   - Imported customer transaction data into a workable format.

2. **Data Cleaning**  
   - Removed missing values, duplicates, and irrelevant entries.

3. **Exploratory Data Analysis (EDA)**  
   - Analyzed customer purchasing behavior, sales patterns, and distribution of key metrics.

4. **Cohort Analysis**  
   - Grouped customers by acquisition month to analyze retention over time.
   - Visualized retention rates using cohort heatmaps.

5. **RFM Feature Engineering**  
   - Built **Recency**, **Frequency**, and **Monetary** features.
   - Added extra features like Customer Lifetime, Average Basket Size, and Total Transactions.

6. **Churn Labeling**  
   - Defined churn as customers with no purchases in the 6 months before the snapshot date.

7. **Predictive Churn Modeling**  
   - Built classification models (Random Forest and XGBoost) to predict customer churn.

8. **Model Evaluation**  
   - Evaluated model performance using metrics like Accuracy, Precision, Recall, F1-score.
   - Saved confusion matrices and classification reports for both models.

---

## How to Run
1. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn xgboost matplotlib seaborn joblib
Run the Jupyter Notebook or Python scripts step-by-step.

Models and evaluation plots will be automatically saved into /models and /evaluations directories.




