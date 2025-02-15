This repository contains the replication study of Unstructured clinical notes within 24 hours to predict 30-day mortality in adult ICU patients. The study employs the MIMIC-III dataset and leverages the XGBoost algorithm for predictive modeling. The project replicates the approach taken by Mahbub et al., focusing on predicting 30-day mortality using clinical notes documented during the first 24 hours of ICU admission.


Key Features:

Replication of the original study by Mahbub et al.
Use of unstructured clinical notes, including Nursing Notes, Discharge Summaries, Radiology Reports, and Physician Notes.
Implementation of natural language processing (NLP) for feature extraction.
Mortality prediction using the XGBoost algorithm.

Methodology
NLP Pipeline
Text Cleaning: Removed stop words, punctuation, and special characters.
Tokenization: Split text into individual tokens for analysis.
Vectorization: Applied TF-IDF to convert unstructured text into structured numerical data.
Model Development
Algorithm: XGBoost (Extreme Gradient Boosting).
Inputs:
Demographic data: Age, gender.
ICU details: Length of stay, interventions.
Preprocessed clinical note vectors.
Hyperparameters:
Learning rate: 0.1
Max depth: 6
Number of estimators: 100
Evaluation Metrics
AUROC Score: 0.85
Precision: 40.5%
Recall: 44.3%
F1-Score: 42.3
