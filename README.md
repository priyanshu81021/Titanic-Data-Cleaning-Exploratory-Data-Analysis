# 🚢 Titanic Data Cleaning & Exploratory Data Analysis (Task-02)

## 📌 Overview
This project is part of the **Prodigy InfoTech Data Science Internship – Task 02**.  
The goal of this task is to perform **Data Cleaning & Exploratory Data Analysis (EDA)** on the **Titanic dataset** to understand the survival patterns of passengers.  

The analysis focuses on handling missing values, engineering new features, and visualizing important relationships between different variables.

---

## 🎯 Objectives
- Perform **data cleaning** (handle missing values & drop irrelevant columns)  
- Create **new features** like *FamilySize* and *IsAlone*  
- Conduct **exploratory data analysis (EDA)** using visualizations  
- Derive meaningful **insights about survival trends**  

---

## 📂 Dataset
The dataset contains details about Titanic passengers, including:
- **Pclass** → Passenger Class (1st, 2nd, 3rd)  
- **Sex** → Gender  
- **Age** → Age of Passenger  
- **SibSp** → Number of Siblings/Spouses aboard  
- **Parch** → Number of Parents/Children aboard  
- **Embarked** → Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  
- **Survived** → Target Variable (0 = Not Survived, 1 = Survived)  

Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)

---

## 🛠️ Steps Performed

### 1. Data Cleaning
- Filled missing **Age** values with median  
- Filled missing **Embarked** values with mode  
- Dropped **Cabin** column due to excessive missing data  
- Engineered new features:  
  - `FamilySize = SibSp + Parch`  
  - `IsAlone = 1 if FamilySize == 0 else 0`  

### 2. Exploratory Data Analysis (EDA)
- Distribution of survival counts  
- Survival analysis by **Gender**  
- Survival analysis by **Passenger Class**  
- Age distribution of survivors vs non-survivors  
- Impact of **Embarkation Port** on survival  
- Role of **Family Size** & **IsAlone** in survival chances  
- Correlation heatmap of numerical variables  
- Combined analysis: **Survival rate by Gender + Pclass**  

---

## 📊 Key Insights
- 🎯 **Gender:** Females had a significantly higher survival rate  
- 🎯 **Passenger Class:** First-class passengers were more likely to survive  
- 🎯 **Age:** Younger passengers had better chances of survival  
- 🎯 **Family Factor:** Medium family sizes had higher survival probability, while solo travelers had lower chances  
- 🎯 **Embarkation Port:** Passengers from Cherbourg (C) showed relatively better survival rates  

---

## ⚙️ Tech Stack
- **Python**  
- **Pandas** → Data manipulation  
- **Matplotlib & Seaborn** → Data visualization  

---

## 📂 Repository Structure
PRODIGY_DS_02/
│── dataset/
│ ├── train.csv
│ ├── test.csv
│ └── gender_submission.csv
│
│── Task02_Titanic_EDA.ipynb
│
│── README.md
│── requirements.txt


---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/priyanshu81021/PRODIGY_DS_02.git

## bash
pip install -r requirements.txt

## bash
jupyter notebook notebooks/Task02_Titanic_EDA.ipynb

---

## 🙌 Internship Info

This project is completed as part of Prodigy InfoTech Data Science Internship – Task 02 (Data Cleaning & EDA).
The task enhanced my skills in:

Data Preprocessing & Cleaning

Exploratory Data Analysis (EDA)

Data Visualization & Insight Generation
