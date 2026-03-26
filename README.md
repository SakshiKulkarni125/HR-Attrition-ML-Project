# HR-Attrition-ML-Project

## Objective
The objective of this project is to build a machine learning model that predicts whether an employee will leave the organization and identify the key factors influencing attrition.

## Business Impact
Employee attrition leads to increased hiring costs, loss of experienced employees, and reduced productivity. This model helps HR teams take proactive steps to retain employees.

---

## Data Understanding
The dataset contains employee-related information including demographics, job role, salary, and satisfaction levels.

### Target Variable:
- Attrition  
  - 1 → Employee will leave  
  - 0 → Employee will stay  

### Key Features:
- Age, Gender, Department  
- Monthly Income  
- Job Satisfaction  
- Work Life Balance  
- Overtime  

---

## Data Cleaning
The following preprocessing steps were performed:

- Removed unnecessary columns:
  - EmployeeNumber  
  - EmployeeCount  
  - Over18  
  - StandardHours  

- Converted categorical variables to numeric  
- Converted boolean values (True/False → 1/0)  
- Checked for missing values  

---

## Exploratory Data Analysis

### Univariate Analysis:
- Age distribution  
- Salary distribution  
- Attrition count  

### Bivariate Analysis:
- Attrition vs Overtime  
- Attrition vs Salary  
- Attrition vs Job Satisfaction  

### Key Observations:
- Employees working overtime are more likely to leave  
- Lower salary leads to higher attrition  
- Poor job satisfaction increases attrition  

---

## Feature Engineering

- Applied Label Encoding to categorical variables  
- Converted all features to numeric format  
- Ensured dataset is ready for modeling  

---

## Model Building

The dataset was split into:
- 80% Training Data  
- 20% Testing Data  

### Models Used:
1. Logistic Regression  
2. Decision Tree  
3. Random Forest  

---

## Model Evaluation

The models were evaluated using:

- Accuracy  
- Confusion Matrix  
- Precision  
- Recall  
- F1 Score  
- ROC-AUC  

### Result:
Random Forest performed best among all models due to its higher accuracy and better generalization.

---

## Confusion Matrix Interpretation

- True Positive: Correctly predicted employee leaving  
- True Negative: Correctly predicted employee staying  
- False Positive: Predicted leaving but stayed  
- False Negative: Predicted staying but left  

Reducing False Negatives is important to avoid losing valuable employees.

---

## Feature Importance

Key factors influencing attrition:

- OverTime  
- MonthlyIncome  
- JobSatisfaction  
- WorkLifeBalance  
- TotalWorkingYears  

---

## Prediction System

The trained model can predict attrition for new employees:

Steps:
1. Input employee details  
2. Apply same encoding  
3. Generate prediction  

Output:
- 0 → Employee will stay  
- 1 → Employee will leave  

---

## Business Insights

- Overtime significantly increases attrition  
- Low salary contributes to employee dissatisfaction  
- Poor work-life balance leads to higher attrition  

---

## Business Recommendations

- Reduce overtime workload  
- Improve salary structure  
- Enhance employee engagement  
- Provide better work-life balance  

---

## Conclusion

This project successfully developed a machine learning model to predict employee attrition.  
Random Forest performed best and provided valuable insights to help HR teams reduce attrition and improve employee retention.
