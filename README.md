# Customer Churn Prediction

##  Project Overview

This project develops a Machine Learning model to predict customer churn in a telecommunications company.

The model analyzes customer demographics, services, contract information, and billing data to predict whether a customer is likely to leave the company.

The project follows an end-to-end Machine Learning workflow, from data exploration and preprocessing to model training, evaluation, and model saving.


##  Business Problem

Customer churn is an important challenge for telecommunications companies because losing customers can negatively affect revenue and long-term growth.

The goal of this project is to build a Machine Learning classification model that can identify customers who are more likely to churn.

---

##  Dataset

This project uses the IBM Telco Customer Churn dataset.

The dataset contains information about customer demographics, services, contracts, payment methods, monthly charges, total charges, and customer churn.

The target variable is `Churn Label`, which indicates whether a customer has churned.

---

##  Project Objectives

* Explore and understand customer data.
* Analyze patterns related to customer churn.
* Prepare the data for Machine Learning.
* Handle missing values and categorical variables.
* Train and compare multiple classification models.
* Evaluate model performance using different metrics.
* Select the most suitable model for customer churn prediction.
* Save the final trained model for future use.

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib
* Google Colab
* GitHub

---

##  Machine Learning Workflow

The project follows these main steps:

1. Data Loading
2. Data Exploration
3. Exploratory Data Analysis (EDA)
4. Data Cleaning
5. Feature Engineering
6. Missing Value Imputation
7. Categorical Feature Encoding
8. Feature Scaling
9. Train-Test Split
10. Model Training
11. Model Evaluation
12. Hyperparameter Tuning
13. Model Selection
14. Model Saving

---

##  Data Preprocessing

The preprocessing pipeline includes:

* Removing irrelevant identifier and location-based features.
* Removing target-related features that could cause data leakage.
* Handling missing numerical values using median imputation.
* Handling missing categorical values using the most frequent value.
* Encoding categorical features using One-Hot Encoding.
* Scaling numerical features using StandardScaler.

---

##  Machine Learning Models

Three classification models were trained and evaluated:

* Logistic Regression
* Decision Tree
* Random Forest

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

---

##  Model Results

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | -------: | --------: | -----: | -------: | ------: |
| Logistic Regression |   80.20% |    64.35% | 56.95% |   60.43% |  84.87% |
| Decision Tree       |   79.42% |    61.60% | 59.63% |   60.60% |  83.57% |
| Random Forest       |   78.78% |    62.63% | 49.73% |   55.44% |  83.28% |

---

##  Final Model

Logistic Regression was selected as the final model based on its overall performance.

It achieved an ROC-AUC score of approximately **84.87%** and an accuracy of approximately **80.20%** on the test set.

Hyperparameter tuning was also performed, but the tuned Logistic Regression model did not improve the original model's performance. Therefore, the original Logistic Regression model was retained as the final model.


##  Project Structure

```text
customer-churn-prediction/
│
├── data/
│   └── Telco_customer_churn.xlsx
│
├── models/
│   └── customer_churn_model.pkl
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── README.md
└── requirements.txt
```

---

##  How to Run

### 1. Clone the repository

```bash
[git clone <repository-url>](https://github.com/EngSaraGamal/Customer-Churn-Prediction)
```

### 2. Install the required libraries

```bash
pip install -r requirements.txt
```

### 3. Open the Jupyter Notebook

Open:

text
notebooks/customer_churn_prediction.ipynb
```

and run the cells in order.

---

##  Future Improvements

Future versions of this project could include:

* Advanced hyperparameter optimization.
* Feature importance analysis.
* Additional Machine Learning models.
* Handling class imbalance using advanced techniques.
* Model deployment using FastAPI or Flask.
* Building a simple web interface for customer churn prediction.

---

##  Author

**Sara**

AI & Machine Learning Enthusiast
