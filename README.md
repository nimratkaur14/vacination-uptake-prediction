# Vaccination Uptake Targeting System for Immunisation Campaigns

## Project Overview
This project uses machine learning to analyse historical influenza vaccination survey data and estimate the probability of two vaccination outcomes: H1N1 vaccination and seasonal influenza vaccination.

## Objectives
- Analyse vaccination uptake patterns in historical survey data.
- Explore demographic, behavioural, healthcare, and opinion-related features.
- Prepare data using missing-value imputation, categorical encoding, and numerical scaling.
- Train and evaluate Logistic Regression models for both vaccination outcomes.
- Compare Logistic Regression and Random Forest for H1N1 prediction.
- Generate vaccination probability estimates for an unlabeled test dataset.

## Dataset
The project uses the Flu Shot Learning: Predict H1N1 and Seasonal Flu Vaccines dataset, containing historical US survey responses from 2009–2010.

The files used are:
- `training_set_features.csv`
- `training_set_labels.csv`
- `test_set_features.csv`

## Methodology
1. Load and merge the survey features and labels.
2. Perform exploratory data analysis.
3. Handle missing values and preprocess numerical and categorical features.
4. Split the labelled data into training and validation sets.
5. Train separate Logistic Regression models for H1N1 and seasonal vaccination.
6. Evaluate model performance using accuracy, precision, recall, F1-score, and ROC-AUC.
7. Experiment with different classification thresholds for H1N1 prediction.
8. Generate probability predictions for the test dataset.

## Key Results
- H1N1 vaccination uptake in the labelled dataset: approximately 21.25%.
- Seasonal influenza vaccination uptake: approximately 46.56%.
- H1N1 Logistic Regression validation ROC-AUC: approximately 0.8287.
- Seasonal Logistic Regression validation ROC-AUC: approximately 0.8552.
- Logistic Regression achieved an H1N1 F1-score of approximately 0.5931 at the experimental threshold of 0.30.

## Project Deliverables
- Google Colab notebook containing the code and analysis.
- Final project report with visualisations.
- `vaccination_uptake_predictions.csv`, containing predicted probabilities for 26,708 test respondents.

## Tools and Libraries
Python, Google Colab, pandas, NumPy, Matplotlib, and scikit-learn.

## Limitations
The dataset reflects historical US survey responses from 2009–2010. Predictions are model estimates, not verified vaccination statuses or medical recommendations. Further validation on representative contemporary data is required before real-world use.

## Future Scope
- Build an interactive dashboard.
- Compare additional machine-learning algorithms.
- Assess probability calibration and performance across population subgroups.
- Evaluate the system using contemporary data and appropriate validation procedures.