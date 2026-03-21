# Data Preparation

Overall Preprocessed Data Shape (7043,13)
Train Preprocessed Data Shape (5634, 13)
Test Preprocessed Data Shape (1409, 13)

## Dataset Overview

The raw dataset contains the following original features:

- gender
- SeniorCitizen
- Dependents
- tenure
- PhoneService
- MultipleLines
- InternetService
- Contract
- MonthlyCharges
- Churn

The target variable is:

- Churn

Churn was transformed as:
- Yes = 1
- No = 0

---

## Numerical Features

The following features were treated as numerical data:

- SeniorCitizen
- tenure
- MonthlyCharges

### Transformation Method
These numerical features were normalised using MinMaxScaler.

### Meaning
- SeniorCitizen:
  - 0 = Not senior citizen
  - 1 = Senior citizen

- tenure:
  - Continuous numerical value representing customer tenure

- MonthlyCharges:
  - Continuous numerical value representing monthly charge amount

---

## Categorical Features

The following features were treated as categorical data:

- gender
- Dependents
- PhoneService
- MultipleLines
- InternetService
- Contract

---

## Binary Encoded Categorical Features

The following categorical features were converted using category codes:

- gender
- Dependents
- PhoneService
- MultipleLines
- InternetService

### Encoding Details

- gender:
  - 0 = Female
  - 1 = Male

- Dependents:
  - 0 = No
  - 1 = Yes

- PhoneService:
  - 0 = No
  - 1 = Yes

- MultipleLines:
  - 0 = No
  - 1 = Yes

- InternetService:
  - 0 = DSL
  - 1 = Fiber optic

---

## One-Hot Encoded Feature

The following categorical feature was transformed using one-hot encoding:

- Contract

### Generated Features
- Contract_Month-to-month
- Contract_One year

### Encoding Meaning
- Contract_Month-to-month:
  - 1 = Month-to-month
  - 0 = Not Month-to-month

- Contract_One year:
  - 1 = One year
  - 0 = Not One year

---
