# 🚗 Vehicle Maintenance Analytics

### Optimizing Vehicle Maintenance Operations Using Data-Driven Analytics

An end-to-end data analytics and machine learning project that explores vehicle maintenance patterns, evaluates classification models, and presents actionable insights through interactive Power BI dashboards.

## 📌 Project Overview

Vehicle maintenance is an important aspect of vehicle reliability and operational planning. This project analyzes vehicle-related data to identify patterns associated with maintenance requirements.

The project combines Python-based data preparation, exploratory data analysis (EDA), feature engineering, machine learning, model evaluation, and Power BI visualization to transform raw data into meaningful insights.

**Dataset size:** 50,000 records  
**Target variable:** `Need_Maintenance`  
- `0` — No maintenance required
- `1` — Maintenance required

## 🎯 Project Objectives

- Prepare and analyze vehicle maintenance data.
- Identify patterns associated with maintenance requirements.
- Explore vehicle condition, reported issues, mileage, and maintenance history.
- Build and evaluate machine learning classification models.
- Develop an interactive Power BI dashboard.
- Communicate findings and acknowledge analytical limitations.

## 🛠️ Tools and Technologies

- **Python** — Data analysis and model development
- **Pandas and NumPy** — Data preparation and numerical analysis
- **Jupyter Notebook** — Analysis workflow and documentation
- **Machine Learning** — Classification and predictive model evaluation
- **Scikit-learn** — Model training and evaluation
- **Power BI** — Interactive dashboards and visual storytelling

## 🔄 Project Workflow

1. **Data inspection:** Examine the dataset structure, variables, and distributions.
2. **Data cleaning and preparation:** Prepare data for analysis and modeling.
3. **Feature engineering:** Create useful derived features, including vehicle age groups and vehicle condition categories.
4. **Exploratory data analysis:** Investigate maintenance patterns across vehicle characteristics.
5. **Machine learning:** Train and compare baseline, Logistic Regression, Decision Tree, and Random Forest classifiers.
6. **Model evaluation:** Assess predictions using accuracy, precision, recall, F1-score, and confusion matrices.
7. **Dashboard development:** Build a three-page Power BI report to communicate analytical findings.

## 📊 Power BI Dashboard

The report contains three pages.

### 1. Maintenance Analysis

- Key performance indicators for vehicle count and maintenance requirements.
- Maintenance patterns across vehicle models and age groups.
- Comparisons across fuel type, transmission type, and maintenance history.

### 2. Vehicle Risk & Condition Analysis

- Maintenance rates across brake, tire, and battery conditions.
- Analysis of reported issues and accident history.
- Comparisons across mileage groups and derived vehicle condition.
- Interactive filters for exploring vehicle categories.

### 3. Diagnostic Insights

- Comparisons involving insurance premium and service recency.
- Maintenance-status distribution across reported-issue categories.
- Ranking factors by observed differences in maintenance rates.
- Summary of important analytical findings.

## 💡 Key Findings

- Approximately **81% of the 50,000 records** were labeled as requiring maintenance.
- Reported issues showed a strong association with maintenance requirements.
- Brake and battery conditions showed substantial differences in maintenance rates across categories.
- Vehicle condition was also associated with maintenance requirements.
- Mileage, tire condition, fuel type, and vehicle age showed relatively small differences in maintenance rates in this dataset.

These findings describe patterns in the available dataset. They do not establish causation or prove that the same relationships will hold in other vehicle populations.

## 🤖 Machine Learning

The project evaluates multiple classification approaches:

- Baseline classifier
- Logistic Regression
- Decision Tree
- Random Forest

The models are compared using accuracy, precision, recall, F1-score, and confusion matrices.

### Model Limitations and Validation

Some tree-based models achieved perfect scores on the original held-out test split. Such results require further investigation and should not automatically be interpreted as evidence of real-world predictive performance.

Additional validation is needed to investigate possible target leakage, understand how the target variable was generated, and evaluate performance on genuinely unseen data.

The models are exploratory and are **not presented as production-ready maintenance decision systems**.

## 📁 Repository Contents

- `vehicle_maintaince(3).ipynb` — Python analysis and machine learning workflow.
- `Vehicle_Maintenance.pbix` — Interactive Power BI report.
- `screenshots/` — Dashboard screenshots.

## 🚀 How to Explore the Project

1. Open the Jupyter Notebook to explore data preparation, analysis, and model evaluation.
2. Review the dashboard screenshots to see the main report pages.
3. Open the `.pbix` file in Power BI Desktop to explore the interactive dashboard.

## 📌 Future Improvements

- Perform further validation of the machine learning models.
- Investigate potential target leakage and target-generation rules.
- Evaluate generalization on additional unseen data.
- Improve model interpretability and error analysis.
- Explore deployment only after the model has been properly validated.

👨‍💻 Author

Vinay D.
BCA Student — Data Science with AI Specialization

I'm building practical skills in data analytics, machine learning, and business intelligence through hands-on projects.

Technical Interests

Data Analytics and Exploratory Data Analysis

Machine Learning and Predictive Modeling

Python, SQL, and Data Visualization

Power BI and Business Intelligence

GitHub: VinayD1402
