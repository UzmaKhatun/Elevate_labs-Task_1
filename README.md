# 🚢 Titanic Dataset - Data Preprocessing Project

This project focuses on cleaning and preprocessing the famous Titanic dataset to prepare it for machine learning tasks such as classification and survival prediction.

## 📂 Dataset Overview

The Titanic dataset provides information on the passengers aboard the Titanic, such as:
- Demographics (age, gender, class)
- Ticket and fare details
- Family relationships aboard
- Survival status

Dataset Source: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic)

---

## 🛠️ Preprocessing Steps

The following data preprocessing steps were performed:

### ✅ Handling Missing Values
- **Age**: Filled using KNN Imputer.
- **Embarked**: Filled using the most frequent value (mode).
- **Fare**: Filled using median or KNN (based on analysis).
- **Cabin**: Dropped due to too many missing values.

### 🔄 Encoding Categorical Features
- **Sex**: Mapped `male → 0`, `female → 1` using LabelEncoder.
- **Embarked**: Mapped `S → 0`, `C → 1`, `Q → 2`.
- **Pclass**: Already numeric.

### 🧹 Dropped Irrelevant Columns
- **PassengerId**, **Name**, **Ticket**, and **Cabin** were dropped as they do not contribute to predictive performance.

---

## 📊 Features After Preprocessing

| Feature        | Type     | Description |
|----------------|----------|-------------|
| `Pclass`       | Numeric  | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| `Sex`          | Numeric  | Gender (0 = male, 1 = female) |
| `Age`          | Numeric  | Age (missing values filled) |
| `SibSp`        | Numeric  | # of siblings/spouses aboard |
| `Parch`        | Numeric  | # of parents/children aboard |
| `Fare`         | Numeric  | Ticket fare |
| `Embarked`     | Numeric  | Port of embarkation (0 = S, 1 = C, 2 = Q) |
| `Survived`     | Binary   | Target variable (0 = No, 1 = Yes) |

---


## 👩‍💻 Author

**Uzma Khatun** – AI/ML Enthusiast  

