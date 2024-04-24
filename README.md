# classification-of-customers

This project focuses on predicting whether a person will purchase vehicle insurance based on various demographic and vehicle-related factors. The goal is to build and evaluate machine learning models to assist in targeted marketing strategies for vehicle insurance providers.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Tools and Libraries Used](#tools-and-libraries-used)
- [Project Structure](#project-structure)
- [Results](#results)
- [Future Improvements](#future-improvements)
## Project Overview

In this project, we conducted exploratory data analysis (EDA), handled missing values, performed feature engineering, and built several machine learning models to predict vehicle insurance purchasing behavior. We addressed class imbalance using the Synthetic Minority Over-sampling Technique (SMOTE) and evaluated model performance using metrics such as accuracy, precision, recall, and AUC-ROC.

## Dataset

The dataset used for this project includes the following columns:

- `Owner Gender`: Gender of the vehicle owner (categorical: 'Male' or 'Female')
- `Owner Age`: Age of the vehicle owner (numerical)
- `Region`: Region of residence (categorical)
- `Vehicle Age`: Age of the vehicle (numerical)
- `Damaged`: Whether the vehicle has been damaged (binary: 'Yes' or 'No')
- `Policy Type`: Type of insurance policy (categorical)

## Methodology

1. **Exploratory Data Analysis (EDA)**:
   - Analyzed data distribution, correlations, and relationships using visualizations (scatter plots, bar plots).

2. **Data Preprocessing**:
   - Handled missing values, converted data types, and performed feature engineering.

3. **SMOTE for Class Imbalance**:
   - Applied SMOTE to address class imbalance in the dataset.

4. **Machine Learning Models**:
   - Built and evaluated multiple models including Logistic Regression, Random Forest Classification, and XGBoost Classification.

## Tools and Libraries Used

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn

## Project Structure
├── data/
│   └── insurance_data.csv
├── notebooks/
│   ├── EDA.ipynb
│   ├── Data_Preprocessing.ipynb
│   ├── Modeling_Logistic_Regression.ipynb
│   ├── Modeling_Random_Forest.ipynb
│   └── Modeling_XGBoost.ipynb
├── src/
│   ├── preprocessing.py
│   └── modeling.py
├── README.md
└── requirements.txt
## Results
Achieved an AUC-ROC score of 0.844 using the best-performing model (Random Forest Classification).
Confusion matrix and classification report are available in the notebook for detailed evaluation.

## Future Improvements
Fine-tune model hyperparameters using grid search or randomized search.
Incorporate additional features or external data sources for improved prediction accuracy.
Deploy the best model as a web application or API for real-time predictions.

