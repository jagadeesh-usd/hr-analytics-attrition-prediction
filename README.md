# HR Analytics Employee Attrition Prediction

This repository contains all code, documentation, and deliverables for our final team project in AAI-510, focused on predicting employee attrition using the IBM HR Analytics dataset.

-----

## Table of Contents

  - [Project Overview](https://www.google.com/search?q=%23project-overview)
  - [Dataset](https://www.google.com/search?q=%23dataset)
  - [Project Structure](https://www.google.com/search?q=%23project-structure)
  - [Business Understanding](https://www.google.com/search?q=%23business-understanding)
  - [Approach](https://www.google.com/search?q=%23approach)
  - [Key Results](https://www.google.com/search?q=%23key-results)
  - [How to Run](https://www.google.com/search?q=%23how-to-run)
  - [Team Contributions](https://www.google.com/search?q=%23team-contributions)
  - [References](https://www.google.com/search?q=%23references)

-----

## Project Overview

Employee attrition is a major challenge for organizations, impacting costs, productivity, and morale. Our project aims to identify key factors influencing attrition and build machine learning models to predict which employees are at risk of leaving. The insights will support HR in developing targeted retention strategies.

-----

## Dataset

  - **Source:** [IBM HR Analytics Employee Attrition & Performance on Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
  - **Records:** 1,470 employees
  - **Features:** 35 columns covering demographics, job satisfaction, compensation, performance, and more.
  - **Target:** `Attrition` (Yes/No)

-----

## Project Structure

```
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
```

-----

## Business Understanding

High employee attrition can signal problems with company culture, compensation, career development, or management practices. By predicting attrition risk and uncovering its drivers, HR can take proactive steps to reduce turnover and retain valuable talent.

-----

## Approach

1.  **Data Understanding & Preparation**
      - Explore dataset, check for missing values, outliers, and inconsistencies
      - Univariate and bivariate analysis of features
2.  **Feature Engineering & Selection**
      - Transform variables as needed
      - Select important features based on correlation and model importance
3.  **Modeling**
      - Train and compare multiple classification models (e.g., Logistic Regression, Decision Tree, Random Forest, XGBOOST)
      - Hyperparameter tuning and model evaluation (Accuracy, ROC-AUC, F1-score)
4.  **Interpretation & Recommendations**
      - Identify top predictors of attrition
      - Provide actionable insights for HR stakeholders
5.  **Deployment Planning**
      - Propose a high-level plan for deploying the model into an HR analytics workflow

-----

## Key Results

  - **Primary Attrition Drivers:** The key factors influencing employee attrition were identified as working **Overtime**, having a **low Monthly Income**, and the specific **Job Role**.
  - **Recommended Model:** An **XGBoost Classifier** was selected as the final model for deployment.
  - **Performance:** The XGBoost model was chosen because it achieved a superior **Recall of 0.60** for the "Attrition = Yes" class. This means it successfully identifies 60% of employees who are at risk of leaving, which directly meets the primary business objective of enabling proactive intervention.

-----

## How to Run

To set up and run this project locally, please follow these steps:

1.  **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/hr-analytics-attrition-prediction.git
    cd hr-analytics-attrition-prediction
    ```

2.  **Create and Activate a Virtual Environment**

    ```bash
    # Create the environment
    python -m venv venv

    # Activate on Mac/Linux
    source venv/bin/activate

    # Activate on Windows
    # venv\Scripts\activate
    ```

3.  **Install Dependencies**
    *(Note: If a `requirements.txt` file is not present, you can generate it from a working environment using `pip freeze > requirements.txt`)*

    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter and Run Notebooks**

    ```bash
    jupyter notebook
    ```

    The notebooks in the `notebooks/` directory are numbered in the recommended order of execution to follow our analytical process:

      - **`00_business_understanding.ipynb`**: Defines the project goals.
      - **`01_data_cleaning.ipynb`**: Prepares the data.
      - **`02_EDA.ipynb`**: Explores the data for initial insights.
      - **`03_A_modeling_RF.ipynb` & `03_B_modeling_XGB.ipynb`**: Detail the training process for each model.
      - **`03_C_model_evaluation.ipynb`**: **This is the key notebook.** It contains the final model comparison, visualization, and our recommendation for deploying the XGBoost model.
      - **`04_model_deployment.ipynb`**: Outlines the production deployment plan.

-----

## License

-----

## Contact