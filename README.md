# ASD-Prediction-in-Children
Machine Learning models for predicting Autism Spectrum Disorder in children aged 4 - 11 years

## Project Overview
This project builds a machine learning pipeline to classify ASD screening outcomes based on behavioral questionnaire data. 
It demonstrates clean data handling, feature inspection, and proper evaluation techniques.

## Data Source
- Dataset: [Autistic Spectrum Disorder Screening Data for Children](https://archive.ics.uci.edu/dataset/419/autistic+spectrum+disorder+screening+data+for+children)  
- The dataset contains behavioral screening responses and demographic information used to classify individuals as ASD or non-ASD.

## Key Steps
1. **Data Wrangling & EDA**  
   - Explored the dataset for missing values and feature distributions.  
   - Removed leakage feature (`result`) to ensure fair evaluation.

2. **Model Development**  
   - Compared Logistic Regression, SVM, and Random Forest using stratified cross-validation.  
   - Pipelines were used for proper scaling and preprocessing.  
   - Final evaluation on the test set included accuracy, recall, F1-score, and ROC-AUC.

## Results
- Best Model: Logistic Regression  
- Test Accuracy: 0.98  
- ROC-AUC: 1.0  

## Key Insights
- Logistic Regression achieved the best performance due to the linear separability of features.  
- Proper feature auditing (removing leakage) is critical for reliable model evaluation.  
- This workflow demonstrates an end-to-end, professional ML pipeline suitable for portfolio presentation.

## Limitations
- The dataset is small, so results may not generalize to a larger population.  
- Features are highly structured and directly related to diagnosis, so performance may be artificially high on this dataset.  
- External validation on independent clinical datasets would be needed for real-world deployment.
