# Fuzzy-Model for Diabetes Classification

This project implements a data-driven fuzzy inference system to aid in the classification of diabetic conditions. The model utilizes variables such as HbA1c and BMI levels to produce an output of diabetes risk status.

---

## 📌 Brief Description

This notebook performs:

- Preprocess data from the diabetes dataset (`diabetes_v2.csv`)
- Fuzzification of HbA1c and BMI variables
- Fuzzy rule definition using `skfuzzy`
- Model evaluation and visualization of fuzzy inference results

---

## 🔧 Features

- Fuzzification of HbA1c (glycated hemoglobin level) and BMI inputs
- ⚙️ Inference using fuzzy control-based IF-THEN rules
- 📉 Visualization of membership functions and defuzzification results
- 📊 Use of XGBoost to compare the results of classical vs fuzzy models

---

## 📂 Input Structure

Main dataset:
- `diabetes_v2.csv`

Columns used:
- `Gender`, `AGE`, `Urea`, `Cr`, `HbA1c`, `Chol`, `TG`, `HDL`, `LDL`, `VLDL`, `BMI`, `CLASS`.

Fuzzy variables:
Input (antecedent)
- **HbA1c**: Low, Normal, High  
- **BMI**: Skinny, Normal, Fat
- **Chol**: Low,Normal,High
Output (consequent)
- **isDiabetes**: True or False
---

## 🛠 Installation

Make sure Python 3.x is installed, then install the dependencies:

``bash
pip install pandas xgboost scikit-learn matplotlib scikit-fuzzy
