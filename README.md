# HR Analytics Employee Attrition Prediction

This repository contains all code, documentation, and deliverables for our final team project in AAI-510, focused on predicting employee attrition using the IBM HR Analytics dataset.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Business Understanding](#business-understanding)
- [Approach](#approach)
- [How to Run](#how-to-run)
- [Key Results](#key-results)
- [Team Contributions](#team-contributions)
- [References](#references)

---

## Project Overview

Employee attrition (voluntary turnover) is a major challenge for organizations, impacting costs, productivity, and morale. Our project aims to identify key factors influencing attrition and build machine learning models to predict which employees are at risk of leaving. The insights will support HR in developing targeted retention strategies.

---

## Dataset

- **Source:** [IBM HR Analytics Employee Attrition & Performance on Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Records:** 1,470 employees
- **Features:** 35 columns covering demographics, job satisfaction, compensation, performance, and more.
- **Target:** `Attrition` (Yes/No)

---

## Project Structure
├── data/                 # Raw and processed datasets
├── notebooks/            # Jupyter notebooks for EDA, modeling, results
├── src/                  # Source code (functions, scripts)
├── resources/
│   ├── data/
│   │   ├── input/                # Raw data
│   │   ├── output/               # Cleaned & processed
│   ├── models/                   # Saved model pipelines (.pkl files)
│       └── ... more models		
├── README.md             # Project documentation

---

## Business Understanding

High employee attrition can signal problems with company culture, compensation, career development, or management practices. By predicting attrition risk and uncovering its drivers, HR can take proactive steps to reduce turnover and retain valuable talent.

---

## Approach

1. **Data Understanding & Preparation**
   - Explore dataset, check for missing values, outliers, and inconsistencies
   - Univariate and bivariate analysis of features

2. **Feature Engineering & Selection**
   - Transform variables as needed
   - Select important features based on correlation and model importance

3. **Modeling**
   - Train and compare multiple classification models (e.g., Logistic Regression, Decision Tree, Random Forest)
   - Hyperparameter tuning and model evaluation (Accuracy, ROC-AUC, F1-score)

4. **Interpretation & Recommendations**
   - Identify top predictors of attrition
   - Provide actionable insights for HR stakeholders

5. **Deployment Planning**
   - Propose a high-level plan for deploying the model into an HR analytics workflow

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/hr-analytics-attrition-prediction.git
cd hr-analytics-attrition-prediction

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```
---

## License

---

## Contact
