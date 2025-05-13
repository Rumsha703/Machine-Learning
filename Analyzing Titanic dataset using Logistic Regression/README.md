# 🚢 Titanic Survival Prediction — Logistic Regression

This project involves analyzing the Titanic dataset to predict passenger survival using **Logistic Regression**. It's a classic binary classification problem widely used to learn data preprocessing, feature engineering, and model evaluation.

---

## 📊 Dataset

The dataset used is the famous [Titanic dataset](https://www.kaggle.com/competitions/titanic/data) from Kaggle, containing information on:

- Passenger demographics (age, gender, class)
- Ticket details
- Survival status

---

## 🧠 Objective

To build a machine learning model that accurately predicts whether a passenger survived the Titanic disaster based on available features.

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas** – data handling
- **NumPy** – numerical operations
- **Matplotlib & Seaborn** – data visualization
- **Scikit-learn** – machine learning

---

## 📈 Key Steps

1. **Data Exploration & Cleaning**
   - Handled missing values
   - Visualized feature relationships

2. **Feature Engineering**
   - Encoded categorical variables (e.g., `Sex`, `Embarked`)
   - Created new features from existing ones

3. **Model Building**
   - Applied **Logistic Regression** from `sklearn`
   - Split data using `train_test_split`
   - Evaluated using accuracy and confusion matrix

4. **Evaluation**
   - Accuracy score
   - Confusion Matrix
   - Classification Report

---

## ✅ Results

The logistic regression model achieved a reasonable prediction accuracy, demonstrating the impact of data cleaning and proper feature engineering. Key insights include:

- **Gender** and **Passenger class** were strong indicators of survival.
- **Missing age values** had to be addressed carefully.
- Logistic regression provided interpretable coefficients.

---



