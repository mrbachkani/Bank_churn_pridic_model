# 🏦 Bank Customer Churn Prediction  

## 📌 Project Overview  
This project predicts **customer churn** (whether a customer will leave the bank) using **machine learning models**. We analyze customer data, identify churn patterns, and build predictive models to help banks retain customers.  

- **Business Goal:** Identify at-risk customers and suggest actions to improve retention.  
- **Tech Stack:** Python, Pandas, Scikit-Learn, XGBoost, Matplotlib, Seaborn  
- **Dataset:** [Bank Customer Churn Dataset (Kaggle)](https://www.kaggle.com/datasets/adammaus/predicting-churn-for-bank-customers)  

---

## 📊 Dataset Description  
The dataset contains **bank customer records** with these key features:  

| **Feature**         | **Description**                           |
|--------------------|----------------------------------|
| `CreditScore`      | Customer's credit score        |
| `Geography`       | Country of residence (France, Spain, Germany) |
| `Gender`          | Male or Female                  |
| `Age`             | Customer’s age                  |
| `Tenure`          | Number of years with the bank  |
| `Balance`         | Account balance                 |
| `NumOfProducts`   | Number of products used        |
| `HasCrCard`       | Credit card ownership (1 = Yes, 0 = No)  |
| `IsActiveMember`  | Activity status (1 = Active, 0 = Inactive) |
| `EstimatedSalary` | Estimated annual salary         |
| `Exited` (Target) | **1 = Churned, 0 = Stayed**    |

---

## 📌 Project Pipeline & Why We Followed This Approach  
| **Step**              | **Action Taken**                        | **Why?** |
|----------------------|--------------------------------|---------|
| **1. Data Preprocessing** | Convert categorical features, handle missing values, scale numerical data | Ensure consistency for model training |
| **2. Exploratory Data Analysis (EDA)** | Visualize churn distribution, correlation analysis | Identify key factors affecting churn |
| **3. Feature Engineering** | Encode categorical variables, drop irrelevant columns | Improve model accuracy |
| **4. Model Training** | Train Logistic Regression, Decision Tree, Random Forest, and XGBoost | Compare different models |
| **5. Model Evaluation** | Check Accuracy, Precision, Recall, F1-Score, ROC-AUC | Ensure the best model for churn prediction |
| **6. Feature Importance Analysis** | Identify key factors influencing churn | Help businesses take action based on insights |
| **7. Model Deployment (Next Step)** | Deploy model using Flask or Streamlit | Allow real-time churn predictions |

---

## 📌 Model Selection & Why We Chose These Algorithms  
| **Algorithm**          | **Why Chosen?**                     | **Best For**               |
|------------------------|--------------------------------|--------------------------|
| **Logistic Regression** | Simple, interpretable baseline model | Small datasets, explainability |
| **Decision Tree**       | Captures non-linear relationships | Quick analysis, easy interpretation |
| **Random Forest**       | Reduces overfitting, better accuracy | Balanced datasets, generalization |
| **XGBoost** (**Best Model**) | High performance, handles imbalanced data | Large datasets, best predictive power |

---
## 📌 How to Run This Project  

### 1️⃣ Clone the Repository  
### 2️⃣ Install Dependencies
### 3️⃣ Run the Jupyter Notebook

## 📌 Model Evaluation & Performance
### ✅ Confusion Matrix: Visualizes correct and incorrect predictions.
### ✅ Precision: Ensures fewer false churn alerts.
### ✅ Recall: Ensures we detect all real churners.
### ✅ ROC-AUC Score: Measures overall model performance.
---
## 📌 Key Takeaways from Evaluation:

## XGBoost achieved the highest accuracy (~89%) and best ROC-AUC score.
## Top churn factors: Age, Account Balance, Number of Products, and Inactive Status.
## Business Insight: High-balance customers are more likely to stay.
---
## 📌 Feature Importance Analysis
### We used XGBoost’s built-in feature importance to understand key factors driving churn.

## 🔹 Top Features Influencing Churn:
### ✔️ Age → Older customers are more likely to leave.
### ✔️ Balance → Higher balance customers tend to stay.
### ✔️ Activity Level → Inactive customers have a higher churn rate.
