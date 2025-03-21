# Diabetes Study Analysis

## 📊 Overview
This project analyzes patterns and predictors of diabetes in Indian women using SQL queries. It explores risk factors such as glucose levels, BMI, cholesterol, and family history to better understand and help prevent diabetes.

## ❤️ Why This Study
I chose this project because both of my parents have diabetes, and I’ve personally witnessed the long-term health complications. This analysis is a step toward understanding the disease more deeply—for my own health and to help others.

## 🧠 Research Questions
*(For corresponding SQL scripts and visualizations, refer to the project folders.)*

- Age distribution in the dataset *(What is the age distribution of the dataset?)*
- BMI distribution *(How does BMI distribution look in the dataset?)*
- WHR across age groups *(How does the Waist-to-Hip Ratio (WHR) vary across different age groups?)*
- Diabetes prevalence *(How common is diabetes in the dataset?)*  
- Family history and glucose *(Do people with a family history of diabetes have higher glucose levels?)*
- LDL/HDL cholesterol differences *(How do LDL and HDL cholesterol levels differ between groups?)*
- LDL > 159 count by group *(How many patients have high LDL by diabetes status?)*
- Medication usage *(What percentage of diabetics take medication?)*
- Strongest predictors *(What are the strongest predictors of diabetes?)*
- Summary statistics *(What are the summary statistics of the dataset?)*
- Diabetes count breakdown *(How many are diabetic vs. non-diabetic?)*
- Average glucose levels *(What is the average glucose level by group?)*
- Risk classification *(How can we build a simple rule to classify risk?)*
- Pregnancy and glucose *(Are pregnant individuals more likely to have higher glucose levels?)*
- Glucose, outcome & BMI *(Analyze the relationship between glucose levels, diabetes outcome, and BMI.)*
- Glucose levels across patient groups *(Rank and calculate running glucose averages.)*

## 🗂️ Repository Structure
```
/diabetes-study-analysis
│
├── data/                     # CSV files used in analysis
├── sql_queries/              # SQL scripts for analysis
├── docs/                     # Reports and detailed summaries
│   └── Diabetes_Study_Summary.md
├── visualizations/           # Images of visualizations
├── README.md                 # Project overview
```

## 📎 Full Report
For the full detailed report and findings, read the [Diabetes Study Summary](docs/Diabetes_Study_Summary.md).

## 💻 How to Explore
1. Load the dataset into your SQL environment (e.g., PostgreSQL, MySQL, SQLite).
2. Run the scripts from the `sql_queries/` folder to explore the data.
3. Review the summary report and visualizations for insights.

## 🔍 Key Insights
- Glucose is the strongest predictor of diabetes.
- BMI correlates with glucose but is not a definitive predictor.
- Family history and cholesterol have limited predictive power.
- Diabetics tend to have more extreme and fluctuating glucose levels.

## 📁 Dataset Features
- Age, BMI, Glucose
- Waist-to-Hip Ratio
- Family History of Diabetes
- LDL, HDL Cholesterol
- Pregnancy, Medication Use
- Diabetes Outcome (1 = Diabetic, 0 = Non-Diabetic)

## 👩‍💻 Author
Personal project motivated by family health history. Aimed at supporting diabetes awareness and early prevention.

## 📜 License
This project is licensed under the MIT License.
