

# HR Analytics Employee Attrition Prediction

This repository contains all code, documentation, and deliverables for our final team project in AAI-510, focused on predicting employee attrition using the IBM HR Analytics dataset.

-----

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Business Understanding](#business-understanding)
- [Approach](#approach)
- [How to Run](#how-to-run)
- [Key Results](#key-results)
- [Team Contributions](#Contact)
- [AI Assistance Disclosure](#ai-assistance-disclosure)
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
├── notebooks/            # Jupyter notebooks for EDA, modeling, results
├── resources/
│   ├── data/
│   │   ├── input/                # Raw data
│   │   ├── output/               # Cleaned & prepared data
│   ├── models/                   # Saved model pipelines 
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
    git clone https://github.com/jagadeesh-usd/hr-analytics-attrition-prediction.git
    ```
    ```bash
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
      - **`Final Project Section1-Team 10.ipynb`**: A single, end-to-end notebook covering business understanding, data preparation, exploratory analysis, modeling (RF & XGBoost), evaluation, and deployment planning for the HR Attrition Prediction project.

-----

## License

-----

## Contact
📩 For any queries or contributions, please reach out to AAI-510 Group 10 (Angshuman Roy ,Daksha S, Jagadeesh Kumar Sellappan).

-----

## AI Assistance Disclosure  
This project follows academic integrity principles by ensuring that all code and analysis reflect a solid grasp of the concepts. AI tools, such as ChatGPT and GitHub Copilot, were utilized for:

**Code Formatting:** Applying PEP 8 standards for improved readability and consistency.

**Commenting:** Improving code documentation with straightforward explanations.

**Debugging Assistance:** Offering guidance on fixing syntax or logical errors.

All outputs generated by AI were thoroughly reviewed, adjusted, and incorporated to guarantee a full understanding and alignment with course goals.
