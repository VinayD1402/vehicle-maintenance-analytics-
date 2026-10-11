# 🚗 Vehicle Maintenance Analytics

### Optimizing Vehicle Maintenance Operations Using Data-Driven Analytics

An end-to-end vehicle maintenance analytics and machine learning portfolio project combining data preparation, exploratory data analysis, feature engineering, predictive model evaluation, and interactive Power BI dashboards.

This project explores vehicle maintenance patterns, evaluates classification models, and transforms analytical findings into interactive visualizations. It also establishes a foundation for future production-level development through model validation, reproducibility, and deployment improvements.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Project Objectives](#-project-objectives)
- [Tools and Technologies](#️-tools-and-technologies)
- [Dataset Overview](#-dataset-overview)
- [Project Workflow](#-project-workflow)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Machine Learning](#-machine-learning)
- [Power BI Dashboard](#-power-bi-dashboard)
- [Key Findings](#-key-findings)
- [Model Limitations and Validation](#-model-limitations-and-validation)
- [Repository Structure](#-repository-structure)
- [How to Explore the Project](#-how-to-explore-the-project)
- [Future Improvements](#-future-improvements-toward-production-level-development)
- [Author](#-author)

---

## 📌 Project Overview

Vehicle maintenance is an important part of vehicle reliability and operational planning. Analyzing vehicle characteristics and maintenance records can help identify patterns associated with maintenance requirements.

This project follows an end-to-end analytical workflow, from preparing the dataset to exploring patterns, developing classification models, evaluating model performance, and communicating findings through Power BI dashboards.

**Project type:** Data Analytics and Machine Learning  
**Dataset size:** 50,000 records  
**Target variable:** `Need_Maintenance`

Target variable interpretation:

- `0` — No maintenance required
- `1` — Maintenance required

The project is intended for learning, analytical exploration, and portfolio demonstration. The current models have not been validated for real-world maintenance decisions.

## 🎯 Problem Statement

How can vehicle-related data be analyzed to identify patterns associated with maintenance requirements, and how can machine learning and interactive dashboards help communicate these patterns?

The project investigates relationships between maintenance requirements and factors such as reported issues, brake condition, battery status, vehicle condition, mileage, maintenance history, and other vehicle characteristics.

## 🎯 Project Objectives

- Inspect and prepare vehicle maintenance data for analysis.
- Perform data cleaning and exploratory data analysis (EDA).
- Engineer useful features from existing vehicle attributes.
- Analyze maintenance rates across vehicle characteristics.
- Develop and compare machine learning classification models.
- Evaluate predictions using multiple classification metrics.
- Build interactive Power BI dashboards for business-oriented analysis.
- Document model limitations and identify improvements needed before production-level use.

## 🛠️ Tools and Technologies

| Technology | Purpose |
|---|---|
| Python | Data analysis and model development |
| Pandas | Data manipulation and preparation |
| NumPy | Numerical operations |
| Jupyter Notebook | Analysis workflow and documentation |
| Scikit-learn | Machine learning and evaluation |
| Power BI | Interactive dashboards and visualization |
| DAX | Measures and calculations in Power BI |

## 📂 Dataset Overview

The project uses a vehicle maintenance dataset containing 50,000 records and 20 original columns.

The dataset includes vehicle characteristics, maintenance-related attributes, and the target variable used for classification.

Examples of analyzed attributes include:

- Vehicle model and age
- Mileage and fuel efficiency
- Fuel type and transmission type
- Brake, tire, and battery condition
- Maintenance history and service recency
- Reported issues and accident history
- Insurance premium
- Maintenance requirement status

The target variable is `Need_Maintenance`.

The results depend on the available dataset and its underlying data-generation process. Findings should not automatically be generalized to all real-world vehicles.

## 🔄 Project Workflow

### 1. Data Inspection and Preparation

- Examined dataset structure, columns, data types, and distributions.
- Prepared data for exploratory analysis and modeling.
- Investigated categorical and numerical attributes.
- Handled date conversion and derived date-related features where applicable.

### 2. Feature Engineering

Created additional features to support analysis, including:

- Vehicle age groups
- Derived vehicle condition categories
- Other useful transformations for exploratory analysis and modeling

### 3. Exploratory Data Analysis

- Compared maintenance rates across vehicle characteristics.
- Investigated patterns in reported issues and component conditions.
- Analyzed categorical distributions and numerical variables.
- Identified variables showing larger or smaller differences in maintenance rates.

### 4. Machine Learning

- Established a baseline for model comparison.
- Trained Logistic Regression, Decision Tree, and Random Forest classifiers.
- Generated predictions on a held-out test split.
- Evaluated the models using classification metrics and confusion matrices.

### 5. Power BI Dashboard Development

- Created a three-page interactive report.
- Designed KPI cards and comparative visualizations.
- Used filters and slicers to explore vehicle categories.
- Presented analytical findings in a business-oriented format.

## 📊 Exploratory Data Analysis

The exploratory analysis focused on understanding how maintenance requirements vary across vehicle characteristics.

Key areas included:

- Maintenance rates by reported-issue count
- Brake and battery condition comparisons
- Vehicle condition categories
- Maintenance history and accident history
- Mileage groups and vehicle age
- Fuel type and transmission type
- Service recency and other available attributes

Maintenance rates were used to compare the proportion of records marked as requiring maintenance across different categories.

## 🤖 Machine Learning

The project treats maintenance requirement prediction as a binary classification problem.

### Models Evaluated

**1. Baseline Classifier**

Provides a reference point for comparing more advanced models.

**2. Logistic Regression**

A linear classification approach used to establish a predictive benchmark.

**3. Decision Tree Classifier**

A tree-based model that learns decision rules from the input features.

**4. Random Forest Classifier**

An ensemble model that combines predictions from multiple decision trees.

### Evaluation Metrics

The models were evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted maintenance cases that were correct.
- **Recall:** Proportion of actual maintenance cases correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion matrix:** Breakdown of correct and incorrect predictions by class.

The goal was to compare model performance rather than select a model based on accuracy alone.

## 📈 Power BI Dashboard

The Power BI report contains three pages designed to present the analysis from different perspectives.

### Page 1 — Maintenance Analysis

Provides an overall summary of the dataset and maintenance patterns.

Includes:

- Total vehicle records
- Vehicles requiring maintenance
- Overall maintenance rate
- Average mileage
- Average fuel efficiency
- Average insurance premium
- Comparisons across vehicle models, age groups, fuel types, transmission types, and maintenance history

### Page 2 — Vehicle Risk & Condition Analysis

Explores the relationship between maintenance requirements and vehicle condition.

Includes:

- Maintenance rates across brake conditions
- Battery and tire condition comparisons
- Derived vehicle condition categories
- Maintenance patterns by reported issues
- Accident history comparisons
- Mileage-group analysis
- Interactive slicers for exploring categories

### Page 3 — Diagnostic Insights

Summarizes additional patterns and comparative findings.

Includes:

- Insurance premium comparisons by maintenance status
- Service-recency analysis
- Maintenance-status distribution across reported-issue categories
- Ranking of factors by observed differences in maintenance rates
- A summary of key analytical findings

These dashboards support exploratory and descriptive analysis. They do not independently establish causation or confirm mechanical faults.

## 💡 Key Findings

The analysis identified the following patterns in the available dataset:

- Approximately **81% of the 50,000 records** were labeled as requiring maintenance.
- Reported issues showed a strong association with maintenance requirements. Higher issue counts generally corresponded to higher maintenance rates.
- Brake condition showed substantial differences in maintenance rates across categories.
- Battery status also showed substantial differences in maintenance rates.
- Vehicle condition categories displayed meaningful differences in maintenance requirements.
- Maintenance history showed differences across its categories.
- Mileage, tire condition, fuel type, and vehicle age showed relatively small differences in maintenance rates in this dataset.

These findings describe associations in the analyzed records. They do not establish causation or guarantee that the same relationships will appear in other vehicle populations.

## ⚠️ Model Limitations and Validation

Some tree-based models achieved perfect scores on the original held-out test split. Such results require careful investigation before being interpreted as evidence of reliable real-world predictive performance.

Important considerations include:

- **Potential target leakage:** Investigate whether any input features directly or indirectly encode the target.
- **Target-generation process:** Understand how `Need_Maintenance` was assigned and whether the input variables overlap with the rules used to create it.
- **Generalization:** Evaluate performance on genuinely unseen data.
- **Class distribution:** Consider the imbalance between the maintenance and no-maintenance classes when interpreting metrics.
- **Practical validity:** Confirm that the required input features would be available before a real maintenance decision.

The models are exploratory and are **not presented as production-ready maintenance prediction systems**. Further validation is required before real-world deployment.

## 📁 Repository Structure

The repository contains the Python notebook, Power BI report, and dashboard screenshots.

```text
vehicle-maintenance-analytics/
├── README.md
├── Vehicle_Maintenance(3).pbix
├── vehicle_maintenance.ipynb
├── Screenshot-1.png
├── Screenshot-2.png
└── Screenshot-3.png
```


## 🚀 How to Explore the Project

### Python Notebook

1. Open the uploaded `.ipynb` notebook on GitHub.
2. Review the data preparation, feature engineering, exploratory analysis, and model evaluation workflow.
3. To execute the notebook locally, install the required dependencies and provide the dataset at the location expected by the notebook.

### Power BI Dashboard

1. Install Power BI Desktop.
2. Download the `.pbix` report from this repository.
3. Open the report in Power BI Desktop.
4. If prompted, configure the data source using the appropriate dataset file.
5. Explore the three report pages and interact with the available slicers.

The Power BI report may require the original dataset or source-path configuration to refresh successfully.

## 🚀 Future Improvements: Toward Production-Level Development

The next stage of this project is to improve reproducibility, validation, reliability, and deployment readiness.

Planned improvements include:

- Investigate potential target leakage and validate the target-generation process.
- Evaluate model performance on genuinely unseen data.
- Build a reproducible preprocessing and model-training pipeline.
- Add systematic validation and error analysis.
- Improve model interpretability and document the selected model.
- Develop a prediction API or interactive application after validating the model.
- Add automated tests, input validation, and appropriate error handling.
- Explore deployment and monitoring of prediction quality and data changes.
- Improve reproducibility and technical documentation.

These are planned improvements, not features claimed as completed in the current version.

## 👨‍💻 Author

**Vinay D.**  
BCA Student — Data Science with AI Specialization

I'm building practical skills in data analytics, machine learning, Python, SQL, and business intelligence through hands-on projects.

### Technical Interests

- Data Analytics and Exploratory Data Analysis
- Machine Learning and Predictive Modeling
- Python, SQL, and Data Visualization
- Power BI and Business Intelligence
- Reliable, end-to-end data science applications


**GitHub:** [VinayD1402](https://github.com/VinayD1402)

I aim to build reliable data science solutions, progressing from exploratory analytics and machine learning experiments toward validated, deployable applications.

---
