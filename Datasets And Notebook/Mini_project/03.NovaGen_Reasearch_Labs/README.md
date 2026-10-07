# NovaGen Health Risk Classification

## 📌 Project Overview

NovaGen Research Labs is conducting large-scale population health studies to better understand how underlying health conditions influence disease risk and long-term health outcomes.

The institute has collected health records from **9,800 individuals** across multiple observational studies. Each record represents a unique participant and contains a combination of numerical and categorical health indicators, including physiological measurements, lifestyle factors, and medical history.

The objective of this project is to develop a **supervised machine learning classification system** that predicts whether an individual is:

- **Healthy**
- **Unhealthy**

The model can support researchers in participant selection and population stratification for clinical trials and longitudinal studies.

---

## 🎯 Problem Statement

Develop a machine learning classification model that can distinguish between healthy and unhealthy individuals using demographic, physiological, lifestyle, and medical-history information.

The prediction can support:

- Selecting eligible participants for clinical trials
- Identifying individuals at higher health risk
- Stratifying populations for risk-based analysis
- Comparing health outcomes across different population groups

---

## 📊 Dataset

The dataset contains health records of **9,800 unique individuals**.

### Features

| Feature | Description |
|---|---|
| `Age` | Age of the individual in years |
| `BMI` | Body Mass Index |
| `Blood_Pressure` | Systolic blood pressure in mmHg |
| `Cholesterol` | Cholesterol level in mg/dL |
| `Glucose_Level` | Blood glucose level in mg/dL |
| `Heart_Rate` | Resting heart rate |
| `Sleep_Hours` | Average sleep hours per day |
| `Exercise_Hours` | Average exercise hours per day |
| `Water_Intake` | Daily water intake in litres |
| `Stress_Level` | Stress level on a predefined scale |
| `Smoking` | Smoking indicator: 1 = Smoker, 0 = Non-smoker |
| `Alcohol` | Alcohol consumption indicator |
| `Diet` | General diet category |
| `MentalHealth` | Mental health score or condition indicator |
| `PhysicalActivity` | Overall physical activity level |
| `MedicalHistory` | Presence of previous medical conditions |
| `Allergies` | Presence of known allergies |
| `Diet_Type__Vegan` | One-hot encoded Vegan diet indicator |
| `Diet_Type__Vegetarian` | One-hot encoded Vegetarian diet indicator |
| `Blood_Group_AB` | One-hot encoded AB blood group |
| `Blood_Group_B` | One-hot encoded B blood group |
| `Blood_Group_O` | One-hot encoded O blood group |

### Target

The target variable represents the individual's health classification:

- `Healthy`
- `Unhealthy`

---

## 🛠️ Machine Learning Approach

This project follows an end-to-end supervised machine learning workflow:

1. Data loading
2. Exploratory Data Analysis (EDA)
3. Data preprocessing
4. Handling categorical variables
5. Feature preparation
6. Train-test split
7. Model training
8. Model evaluation
9. Comparison of multiple classification algorithms
10. Selection of the best-performing classifier

---

## 🤖 Models Used

The following classification algorithms were evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random