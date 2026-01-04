# Rainfall Prediction in Melbourne Using Machine Learning

## Overview
This project builds an end-to-end machine learning pipeline to predict whether
it will rain on a given day in the Melbourne region using historical weather data.
The goal is to demonstrate practical machine learning skills including feature
engineering, model pipelines, hyperparameter tuning, and evaluation.

## Problem Statement
Accurate rainfall prediction is important for daily planning and risk management.
Using historical meteorological data, this project predicts whether measurable
rainfall will occur on a given day.

## Dataset
The dataset contains daily weather observations from Australia between 2008 and 2017.

**Sources:**
- Australian Bureau of Meteorology (BOM)
- Kaggle: Weather Dataset (Rattle Package)

The analysis focuses on the following locations to reduce geographic variability:
- Melbourne
- Melbourne Airport
- Watsonia

## Key Challenges Addressed
- Handling missing data
- Preventing data leakage by redefining the prediction target
- Managing categorical and numerical features
- Class imbalance in rainfall prediction

## Feature Engineering
- Dropped features with excessive missing values
- Renamed rainfall labels to avoid target leakage
- Engineered a seasonal feature from date information
- Filtered data by geographically close locations

## Modeling Approach
Two supervised classification models were implemented and compared:

### 1. Random Forest Classifier
- Robust to feature interactions
- Tuned using GridSearchCV
- Achieved strong overall accuracy

### 2. Logistic Regression
- Interpretable baseline model
- Improved recall for rainy days
- Better performance on minority class prediction

Both models were trained using a unified preprocessing and modeling pipeline.

## Evaluation Metrics
- Accuracy
- Precision, Recall, and F1-score
- Confusion Matrix
- Feature Importance (Random Forest)

## Results
- Overall accuracy: ~84%
- Logistic Regression showed slightly better recall for rainfall events
- Seasonal patterns and humidity-related features were among the most influential

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Project Structure

```text
rainfall-prediction-melbourne/
│
├── rainfall_prediction_melbourne.ipynb
├── README.md
├── requirements.txt
```


## How to Run

1. Clone the repository

```bash
    git clone https://github.com/amarkumar55/rainfall-prediction-melbourne.git
   
```

###  Install dependencies
    
    pip install -r requirements.txt
   
### Run the notebook
    
    jupyter notebook rainfall_prediction_melbourne.ipynb


### Disclaimer
    This project was completed independently as part of my learning journey.
    All code, analysis, and explanations are my own.


### Author

### Amar Kumar
### LinkedIn: https://www.linkedin.com/in/amarinfo
### GitHub: https://github.com/amarkumar55
