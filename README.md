# 🚢 Titanic Survival Prediction

This project predicts whether a passenger survived the Titanic disaster using machine learning. It applies data preprocessing, feature engineering, and classification models to achieve accurate survival predictions.

## 📌 Project Overview

Dataset: Titanic dataset (Kaggle / open-source)

Goal: Predict survival (0 = Not Survived, 1 = Survived)

Approach: Data cleaning → Feature engineering → Model training → Evaluation

## ⚙️ Tech Stack

Python (pandas, numpy, scikit-learn, matplotlib, seaborn)

Jupyter Notebook / Google Colab

## 🗂 Dataset Features

Pclass: Ticket class (1, 2, 3)

Sex: Gender of passenger

Age: Age in years

Fare: Ticket fare

SibSp: # of siblings/spouses aboard

Parch: # of parents/children aboard

Embarked: Port of embarkation (C, Q, S)

Survived: Target variable (0 or 1)

## 🔑 Key Steps

### Data Preprocessing

Handle missing values (median for Age, mode for Embarked)

Drop irrelevant columns (PassengerId, Ticket, Cabin)

### Feature Engineering

Created FamilySize = SibSp + Parch

One-hot encoding for categorical variables (Sex, Embarked)

### Model Training

Logistic Regression / Random Forest / Decision Tree

Evaluated using confusion matrix & accuracy score

Sample Prediction

Input:  Pclass=2, Sex=female, Age=28, Fare=15.0, FamilySize=1  
Output: Survived ✅ (Prediction Probability ~ 86%)  

### 📊 Results

Best model accuracy: 81%

Insights:

Females and children had higher survival rates

Higher-class passengers had better chances

### 🚀 How to Run

Clone the repo

git clone https://github.com/272006Sakshi/titanic-survival-prediction.git
cd titanic-survival-prediction


Install dependencies

pip install -r requirements.txt


Run Jupyter Notebook 

jupyter notebook Titanic_Prediction.ipynb
# or
streamlit run app.py

📌 Future Improvements

Try deep learning models (ANNs)

Deploy using Flask / Streamlit

Add visual dashboards
