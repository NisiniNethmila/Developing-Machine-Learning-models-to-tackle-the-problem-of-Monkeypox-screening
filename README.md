# MonkeyPox Prediction Using Machine Learning
A machine learning-based predictive analytics project focused on identifying potential Mpox (MonkeyPox) infections using patient symptom data. This project explores multiple supervised learning algorithms to develop a cost-effective screening approach that can reduce dependency on PCR testing.

## Project Overview
This project investigates whether machine learning models can accurately predict Mpox infections based on clinical symptoms and patient characteristics. The goal is to support faster and more affordable screening processes, especially in situations where PCR testing is expensive or time-consuming.

The project includes:
- Data preprocessing and feature engineering
- Exploratory Data Analysis (EDA)
- Data visualisation
- Training and evaluation of multiple ML models
- Hyperparameter tuning and model optimisation
- Comparative performance analysis

## Objective
- Predict Mpox infection status using symptom-based data
- Reduce the need for expensive PCR tests
- Compare multiple machine learning classification algorithms
- Identify the best-performing predictive model
- Improve healthcare decision-making using data analytics
  
## Dataset Information
The dataset contains clinical characteristics of patients during the 2022 Mpox outbreak.

Dataset Features

| Feature                        | Type    |
| ------------------------------ | ------- |
| Patient_ID                     | Object  |
| Systemic Illness               | Object  |
| Rectal Pain                    | Boolean |
| Sore Throat                    | Boolean |
| Penile Oedema                  | Boolean |
| Oral Lesions                   | Boolean |
| Solitary Lesion                | Boolean |
| Swollen Tonsils                | Boolean |
| HIV Infection                  | Boolean |
| Sexually Transmitted Infection | Boolean |
| MPOX PCR Result                | Object  |


Dataset Source

[Kaggle](https://www.kaggle.com/datasets/muhammad4hmed/monkeypox-patients-dataset)


## Technologies & Libraries Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

### Development Environment
- Jupyter Notebook
  
## Exploratory Data Analysis (EDA)

The project includes several visualisations and statistical analyses to better understand the dataset:

- Distribution of systemic illnesses
- Symptom frequency analysis
- MonkeyPox positive vs negative distribution
- Missing value analysis
- Feature distribution analysis
  
## Data Preprocessing

The following preprocessing steps were applied:

- Handling Missing Values
Removed rows containing missing values using dropna()

- Feature Selection
Removed Patient_ID column to preserve anonymity and eliminate unnecessary features

- Encoding
Converted categorical and Boolean features into numerical format using LabelEncoder

- Train-Test Split
Dataset split into:
  - 80% Training
  - 20% Testing
  
## Machine Learning Models Used

The following classification algorithms were implemented and evaluated:

- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbour (KNN)
- Logistic Regression
- Decision Tree
- Gradient Boosting
- XGBoost


## Hyperparameter Optimisation

Hyperparameter tuning was performed using:

- GridSearchCV
- RandomizedSearchCV

This helped improve model performance and identify optimal parameters for each algorithm.

## Model Performance

| Model               | Accuracy After Optimization |
| ------------------- | --------------------------- |
| Random Forest       | 69%                         |
| SVM                 | 72%                         |
| KNN                 | 69%                         |
| Logistic Regression | 70%                         |
| Decision Tree       | 69%                         |
| Gradient Boosting   | 72%                         |
| XGBoost             | 72%                         |


### Best Performing Models

- Support Vector Machine (SVM)
- Gradient Boosting
- XGBoost

All achieved approximately 72% accuracy after hyperparameter optimisation.

## Key Findings

- Machine learning models can effectively predict potential Mpox infections using symptom data.
- Gradient Boosting, SVM, and XGBoost showed the best predictive performance.
- The project demonstrates the potential of AI-assisted disease screening systems.
- Data preprocessing significantly impacted model performance and dataset quality.

## Challenges & Limitations
- Approximately 25% of the dataset contained missing values
- Reduced dataset size after preprocessing
- Limited number of features
- Privacy and ethical concerns with healthcare data
- Model accuracy may improve with larger and more diverse datasets

## Project Structure

├──           # Python code
├── README.md  
├──                     # Data file
└──      # Report

```text
.
├── MDA512_Assignment2_Group1.pdf      # Report
├── MonkeyPox_Analysis.ipynb           # Training/experiment notebooks
├── monkeypox.csv                      # Data file
└── README.md
```



## Report
[View](MDA512_Assignment2_Group1.pdf)


## How to Run
1. Clone the repository.
2. Install Required Libraries.
3. Run the Jupyter Notebook.

## Future Improvements
- Use larger healthcare datasets
- Improve feature engineering
- Apply deep learning techniques
- Build a real-time prediction dashboard
- Deploy the model using Streamlit or Flask

## Contributors
- **Sandeep Karmacharya**
- **Chimi Wangmo**
- **Nisini Silva**
- **Dewmini Aranayake**
