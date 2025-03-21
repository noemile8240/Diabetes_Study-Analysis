# Diabetes of Indian Women Study Analysis

## Overview
This project uses data originally downloaded from Kaggle. This study was conducted exclusively on Indian women and focuses on identifying patterns and predictors of diabetes. The dataset includes various health indicators such as age, BMI, glucose levels, cholesterol levels, and more.  
If you would like to see the visualization plots for this study, please reference the project **Visualization of Diabetes Study of Indian Women.**

## Why This Study Was Chosen
I chose to work on this diabetes study because both of my parents have diabetes, and I have personally witnessed the consequences and health complications that come with it. This project is more than just an analysis—it is a way for me to gain deeper insights into the disease, understand the key risk factors, and find ways to prevent it for myself and others. By studying these patterns, I hope to contribute to a better understanding of diabetes and its early prevention.

## Research Questions Addressed
*(If you want to see the visualizations related to these research questions, please refer to the corresponding scripts where the data is analyzed and visualized.)*

- Age distribution in the dataset *(What is the age distribution of the dataset?)*
- BMI distribution *(How does BMI distribution look in the dataset?)*
- Waist-to-Hip Ratio (WHR) across age groups *(How does the Waist-to-Hip Ratio (WHR) vary across different age groups?)*
- Diabetes prevalence in the dataset *(How common is diabetes (Outcome = 1) in the dataset?)*
- Impact of family history on glucose levels *(Do people with a family history of diabetes have higher glucose levels?)*
- LDL and HDL cholesterol differences between diabetic and non-diabetic individuals *(How do LDL and HDL cholesterol levels differ between those with and without diabetes?)*
- LDL > 159 count for Diabetic vs. Non-Diabetic patients *(How many Diabetic and Non-Diabetic patients have LDL > 159?)*
- Diabetes medication usage *(What percentage of individuals with diabetes take medication?)*
- Strongest predictors of diabetes *(What are the strongest predictors of diabetes?)*
- Summary statistics of the dataset *(What are the summary statistics of the dataset?)*
- Diabetes count breakdown *(How many patients are diabetic (Outcome = 1) and non-diabetic (Outcome = 0)?)* 
- Average glucose levels for diabetics and non-diabetics *(What is the average glucose level for diabetics and non-diabetics?)*
- Diabetes risk classification *(How can a simple rule be built to classify diabetes risk?)*
- Effect of pregnancy on glucose levels *(Are pregnant individuals more likely to have higher glucose levels?)*
- Glucose levels, diabetes outcome, and BMI relationship *(Analyzing the relationship between glucose levels, diabetes outcome, and BMI.)*
- Glucose levels across patient groups while ranking and calculating running averages *(Analyze glucose levels across different patient groups while ranking them and calculating running averages.)*

## Key Findings

### Age Distribution
- The age bracket with the highest patient count is 34, followed by 71 and 43.

### BMI and Diabetes Outcome
- The obese category (BMI > 29.9) has the highest diabetes onset.
- The underweight category (BMI < 18.5) has the lowest count.
- BMI has a weak correlation (0.11) with diabetes, indicating that BMI alone is not a strong predictor.
- While higher BMI is associated with increased glucose levels, it does not reliably indicate diabetes status.

### Waist-to-Hip Ratio (WHR)
- Minimal variation across age groups.
- The senior age group has the highest average (0.92), while the very young group has the lowest (0.91).

### Diabetes Prevalence
- 34% of patients in the dataset are diabetic (3,282), while 66% are non-diabetic (6,256).

### Family History and Glucose Levels
- Family history does not significantly impact glucose levels.
- Average glucose levels:
  - Family history = 0 → 106.18
  - Family history = 1 → 105.93

### LDL & HDL Cholesterol Levels
- Diabetic Patients: LDL = 100.94, HDL = 49.77
- Non-Diabetic Patients: LDL = 99.71, HDL = 50.05
- Patients with LDL > 159:
  - Non-Diabetic = 162
  - Diabetic = 78

### Diabetes Medication Usage
- Diabetic patients taking medication: 44.88%
- Non-diabetic patients taking medication: 38.20%

### Strongest Predictors of Diabetes
- Glucose levels are the most significant predictor.
- Non-diabetics have a higher median glucose rank (~3116) compared to diabetics (~1641).
- Higher glucose ranks are predominantly in non-diabetics, which is an unexpected finding.
- There is a moderate correlation (0.56) between glucose levels and BMI, indicating individuals with higher BMI tend to have higher glucose levels.

### Glucose and Diabetes Outcome
- There is a weak positive correlation (0.17) between glucose levels and diabetes diagnosis.
- Most diabetic individuals have glucose levels above 140.
- In the mid-range glucose levels (~100-140), both diabetic and non-diabetic cases are present, indicating multiple factors contribute to diabetes risk beyond glucose and BMI alone.
- Individuals with diabetes tend to have glucose levels that cluster in higher ranges, reinforcing the importance of glucose monitoring in early detection and management.

### Glucose Levels Across Patient Groups with Ranking and Running Averages
1. **Diabetic Patients Have Higher Average Glucose Levels**  
   - The average glucose level for non-diabetic patients is 103.43, while for diabetic patients, it is 111.20.

2. **Median Glucose Levels Are Close for Both Groups**  
   - The median glucose level is 104.5 for non-diabetics and 109.5 for diabetics.

3. **Glucose Levels in Diabetics Have a Wider Range**  
   - The minimum glucose level is 50.0 for both groups.
   - The maximum glucose level for diabetics is 207.2, compared to 140.0 for non-diabetics.

4. **Running Averages Suggest Higher Fluctuations in Glucose Levels for Diabetics**  
   - Average running glucose for non-diabetics: 85.38  
   - Average running glucose for diabetics: 89.07

## Conclusion
This study highlights the significant correlation between glucose levels and diabetes while showing that BMI, cholesterol, and family history play a lesser role. The findings help define potential risk categories for diabetes prediction and provide insight into medication usage trends among diabetic individuals. Additionally, the moderate correlation between glucose and BMI suggests that obesity is associated with increased glucose levels, though BMI alone is not a definitive predictor of diabetes.

Further analysis could focus on additional lifestyle factors, genetic predisposition, and dietary habits that may contribute to diabetes onset.
