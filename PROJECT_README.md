
# Understanding Diabetes Risk Through Multi-Factor Analysis

## Table of Contents
- [Project Background](#project-background)  
- [Data Structure & Initial Checks](#data-structure--initial-checks)  
- [Executive Summary](#executive-summary)  
- [Insights Deep Dive](#insights-deep-dive)  
  - [Glucose Thresholds](#glucose-threshold-analysis)  
  - [Demographic Age](#demographic-impact-age)  
  - [Biometric Risk Correlation](#biometric-risk-correlation)  
  - [Combined Risk Factors](#combined-risk-factors)  
  - [Correlation Matrix](#correlation-matrix)  
- [Recommendations](#recommendations)  
- [Assumptions & Caveats](#assumptions--caveats)  
- [Technical Resources & Links](#technical-resources--links)  

---

## Project Background

Elist Health is a healthcare analytics organization focused on improving early detection of chronic conditions through data. This project analyzes health records to identify biometric indicators strongly correlated with diabetes risk. The dataset includes anonymized health and demographic information on over 9,000 women patients.

The project leverages SQL and Tableau to explore data patterns, validate statistical relationships, and communicate insights visually. Key objectives include:

- Identifying biometric variables most predictive of diabetes  
- Uncovering threshold-based risk patterns (e.g., glucose, BMI)  
- Providing actionable recommendations to guide screening strategies  

Insights and recommendations are delivered in the following key areas:

- **Glucose Thresholds:** Analysis of diabetic prevalence across glucose levels to identify high- and low-risk ranges  
- **Demographic Impact:** Examining age-based diabetes patterns in both proportion and volume  
- **Biometric Risk Correlation:** Investigating variable relationships (e.g., glucose vs. BMI) to identify compounding factors  
- **Multi-variable Interactions:** Exploring the combined impact of age, BMI, and glucose  

---

## Data Structure & Initial Checks

The original dataset consisted of a single table with demographic and biometric data from 9,538 individuals. To enhance clarity and facilitate analysis, the data was restructured into two logical tables during the preparation phase.

- **patients:** Includes PatientID, age, number of pregnancies, blood pressure, BMI, medication use, diabetes pedigree function, and diabetes outcome (positive/negative).  
- **lab_results:** Contains glucose level, HBA1c, LDL, HDL, Triglycerides, Waist Circumference, Hip Circumference, WHR (Waist Hip Ratio).

To support segmentation and dashboard filtering, additional fields were created:

- **Age Group:** Categorizes patients into age brackets (e.g., 20–29, 30–39) for easier comparison.  
- **BMI Category:** Classifies BMI values into standard groups (Underweight, Normal, Overweight, Obese).  
- **patientID and labID:** Introduced to uniquely identify individuals and associate lab results.

**SQL** played a key role in the early stages of analysis by enabling:

- Data cleansing (handling zeros and duplicates)  
- Summary metric calculations (e.g., average glucose by age group)  
- Distribution comparisons across diabetic and non-diabetic groups  
- Identification of high-risk indicators through exploratory queries  
- Segmentation by glucose ranges, BMI categories, and age brackets  

**Tableau** was then used to bring the analysis to life through interactive visualizations and dashboards. Additional calculated fields were created within Tableau to support threshold analysis, enhance user filtering, and surface patterns across key health indicators.

Together, SQL and Tableau created a seamless workflow from raw data to actionable insights — ensuring both analytical accuracy and accessible storytelling.

---

## Executive Summary

### Overview of Findings

This analysis uncovered clear and actionable patterns in the relationship between biometric health indicators and diabetes risk. The most significant predictors include elevated glucose levels, high BMI, and age over 40 — all of which show strong individual and combined effects. Correlation trends between glucose, BMI, and blood pressure further support the presence of compounding risk factors.

The findings suggest meaningful opportunities for healthcare teams to improve early detection strategies and prioritize screening efforts for high-risk populations, particularly older individuals and those presenting with elevated glucose or BMI. These insights can also inform more targeted education and intervention programs.

To support these insights, the project leveraged both SQL and Tableau:

- **SQL** was used to explore statistical relationships, calculate summary metrics, validate data quality, and examine subgroup behaviors.  
- **Tableau** provided a visual layer to interpret trends and communicate insights effectively via dashboards and exploratory charts.

### Key Trends and Findings

- **Elevated Glucose = Higher Risk:** Patients with glucose levels >120 mg/dL had a significantly higher rate of diabetes positivity.  
- **BMI Matters:** Individuals classified as Obese (BMI >30) were substantially more likely to be diabetic.  
- **Age Correlation:** Diabetes prevalence increased notably among those aged 40 and older.  
- **Compounding Risk:** Patients with both high BMI and high glucose levels represented the most at-risk group.  
  - Among patients aged 70+ with both high glucose (126+) and high blood pressure (130+), diabetes rates exceeded 85%.  
  - In the severely obese BMI group (BMI ≥35), diabetes risk surpassed 68% in patients over 70.  
  - Even with normal glucose and blood pressure, diabetes prevalence increased from ~29% in the 40s to over 39% in the 70+ age group.  

These combined insights support the use of stacked biomarker thresholds for smarter, more targeted screening.

---

## Insights Deep Dive

### Glucose Threshold Analysis

Glucose Levels and Diabetes: Patients with glucose levels in the diabetic range (≥126 mg/dL) consistently had the highest diabetes rates, especially in older age groups. Across all ages, glucose emerged as the most directly predictive metric of diabetes status. Among patients aged 70+ with glucose in the diabetic range, more than 57% had diabetes. Even within "normal" glucose ranges, risk increased steadily with age.

- Diabetic prevalence peaks in the 90–110 range, with diabetic patients making up over 14% of the group.

### Demographic Impact (Age)

Age as a Risk Factor: Diabetes risk rises steadily with age, with notable increases in the 60–69 and 70+ groups. Even among patients with normal glucose and blood pressure, diabetes prevalence climbs from ~29% in patients in their 40s to over 39% in those aged 70+. Age alone is a meaningful flag for screening.

- Patients aged 70+ with both diabetic glucose and high blood pressure had diabetes rates over 85%.  
- Prediabetic individuals (glucose 100–125) with normal BP still showed 25–30% diabetes prevalence in older age bands.

### Biometric Risk Correlation

- Glucose and BMI show a strong positive correlation, especially among diabetic patients.  
- **BMI Group Analysis:** Obese and severely obese individuals had markedly elevated diabetes rates. Among severely obese patients aged 70+, 68% were diabetic.  
- Rates climbed progressively across BMI brackets, even within the same age group — supporting the inclusion of BMI as a major contributor to risk stratification.

### Combined Risk Factors

- **High BMI + Glucose yields the highest standalone risk**  
- **Systolic BP and glucose → Big spike in older adults**  
- Age and blood pressure also trend together in diabetic patients.  
- Average blood pressure increases with age for all individuals, but diabetic patients consistently show higher readings — highlighting a compounded cardiovascular risk in older populations.  
- These risk factors interact and amplify one another, underscoring the need for multifactor screening protocols.

### Correlation Matrix

To wrap up the analysis, the correlation matrix below illustrates the strength of relationships among key health indicators — glucose, BMI, age, and blood pressure.

- Notably, BMI & blood pressure (0.61) and glucose & BMI (0.56) show strong positive correlations, pointing to compound risk factors.  
- This visual supports the earlier insights by highlighting how certain variables tend to increase together, reinforcing where the most impactful risk interactions occur.

---

## Recommendations

- Prioritize glucose screening for individuals with glucose levels over 120 mg/dL — this threshold marks a steep increase in risk.  
- Target individuals with BMI >30, particularly when paired with elevated glucose.  
- Focus education and screening on patients aged 40+, especially those in the 60–90 age range.  
- Develop integrated risk flags for patients showing both high glucose and high BMI — this subgroup is the most at-risk.  
- Use correlation insights (glucose + BMI + BP) to guide comprehensive risk prediction models.  
- Leverage correlation-based thresholds for targeted risk alerts in dashboards. Introduce layered screening protocols using age + glucose + BP/BMI.  
- Prioritize patients over 60 when two or more biomarkers are elevated.

> See the accompanying Tableau dashboard for visual summaries of these insights.

---

## Technical Resources & Links

- **SQL Queries – Data Exploration & Cleaning**  
- **SQL Queries – Summary Metrics & Segmentation**  
- **Tableau Dashboard Link**  
- **Entity Relationship Diagram (ERD)**

---

## Assumptions & Caveats

- The dataset represents a simulated patient population and may not reflect clinical diversity.  
- Insulin values were excluded due to data quality issues, though knowing whether a patient was actively taking insulin on the day of lab readings would be clinically relevant.  
- No time series or longitudinal tracking was available — all data is cross-sectional.  
- All metrics represent a single-day snapshot, not longitudinal tracking.  
- Visualizations are based on grouped bins and aggregated statistics, which may mask individual variability.
