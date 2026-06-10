# Diabetes Patient EDA — Pima Indians Dataset

## Overview
An end-to-end Exploratory Data Analysis project on the Pima Indians 
Diabetes. Dataset containing 768 female patients. This project covers 
data cleaning, statistical analysis, and visualization to identify key diabetes risk factors.

## Dataset
- Source: National Institute of Diabetes and Digestive and Kidney Diseases
- Rows: 768 patients | Columns: 9
- Features: Pregnancies, Glucose, BloodPressure, SkinThickness, 
  Insulin, BMI, DiabetesPedigreeFunction, Age, Outcome

## Key Findings
1. Glucose is the strongest predictor of diabetes with a correlation 
   of 0.49 with Outcome
2. Nearly 49% of Insulin values were hidden as impossible zero values 
   — discovered and handled through median imputation
3. Patients in the diabetic glucose range (126+) had a 70%+ diabetes rate
4. Senior patients (46+) showed significantly higher diabetes rates 
   than younger age groups
5. Obese patients (BMI 30+) had the highest diabetes rate across all 
   BMI categories

## Data Quality Issues Found
- 5 columns contained medically impossible zero values
- Insulin: 374 missing values (48.7%) hidden as zeros
- SkinThickness: 227 missing values (29.6%) hidden as zeros
- Handled by replacing zeros with NaN then median imputation

## Tools Used
- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scipy (statistical testing)
- Jupyter Notebook

## Project Structure
- Diabetes_patient_EDA_project.ipynb — main analysis notebook
- pima_indians_diabetes.csv — dataset

## How To Run
git clone https://github.com/bikashsahani/diabetes-patient-eda.git
cd diabetes-patient-eda
pip install pandas numpy matplotlib seaborn scipy
jupyter notebook
