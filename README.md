# Heart Disease Prediction

## CSCA 5622: Intro to Machine Learning - Supervised Learning final project

This project implements supervised machine learning models to predict the presence of heart disease in patients using the UCI Heart Disease dataset.

## Project Overview

Heart disease remains one of the leading causes of death globally. This project aims to:
1. Develop a predictive model for early detection of heart disease
2. Compare multiple algorithms to find the best approach
3. Identify medical factors that contribute to heart disease

## Dataset

The UCI Heart Disease dataset contains medical attributes from patients including:
- Age, sex, and other demographic information
- Clinical measurements (blood pressure, cholesterol levels, etc.)
- Results from various medical tests
- Presence or absence of heart disease

The dataset was collected from several sources, including the Cleveland Clinic Foundation.

## Methodology

This project follows a comprehensive machine learning workflow:

1. **Exploratory Data Analysis (EDA)**
   - Statistical analysis of features
   - Visualization of distributions and relationships
   - Correlation analysis

2. **Data Cleaning and Preprocessing**
   - Missing value detection and imputation
   - Outlier identification and treatment
   - Feature scaling and transformation

3. **Feature Engineering**
   - Creation of new derived features
   - Feature selection based on importance

4. **Model Development**
   - Implementation of multiple algorithms:
     - Logistic Regression
     - Random Forest
     - Support Vector Machine (SVM)
     - XGBoost
   - Cross-validation
   - Hyperparameter tuning

5. **Model Evaluation**
   - Performance metrics comparison
   - ROC curve analysis
   - Feature importance assessment

## Results

- The best performing model achieved an accuracy of 85.53% on the test set
- Key predictive features include  thallium stress test results (thal), number of major vessels (ca), chest pain type (cp)
- The model demonstrates significant potential for clinical application

## Structure

```
heart-disease-prediction/
├── data/
│   ├── raw/              # UCI Heart Disease dataset
├── models/               # Saved trained models
├── heart_disease_analysis.ipynb  # Main Jupyter notebook with analysis
├── README.md             # This file
└── requirements.txt      # Dependencies
```

## Setup and Usage

1. Clone this repo
   ```bash
   git clone https://github.com/rylanturner02/heart-disease-prediction.git
   cd heart-disease-prediction
   ```

2. Create a virtual environment and install dependencies
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook
   ```bash
   jupyter notebook heart_disease_analysis.ipynb
   ```

## Dependencies

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost

## Reference

1. UCI Machine Learning Repository: Heart Disease Dataset
   https://archive.ics.uci.edu/dataset/45/heart+disease

## Author

Rylan Turner

## License

This project is licensed under the MIT License.
