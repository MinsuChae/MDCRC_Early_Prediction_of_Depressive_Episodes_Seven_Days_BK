# README

## Study Overview

We conducted a study in South Korea involving patients diagnosed with depression as well as those with mania or hypomania. Diagnoses were made by licensed clinicians in accordance with the criteria outlined in the *Diagnostic and Statistical Manual of Mental Disorders, Fifth Edition (DSM-5)*. The study was approved by the Institutional Review Board (IRB) of "[ClinicalTrials.gov: NCT03088657](https://clinicaltrials.gov/study/NCT03088657)".

## Data Collection and Features

Physiological data were collected using Fitbit devices worn by patients, while light exposure patterns were recorded via a custom Android application.  
The features used in this study included:

- Step count  
- Heart rate  
- Sleep information  
- Light exposure patterns

Details regarding the preprocessing of these features can be found in the files within the `preprocessing` directory. Feature selection was performed using chi-square tests and t-tests, in collaboration with clinical experts. The final set of variables used for analysis is documented in the [`preprocessing/preprocessing_file_merge.ipynb`](https://github.com/MinsuChae/MDCRC_Early_Prediction_of_Depressive_Episodes_Seven_Days_BK/blob/main/preprocessing/preprcessing_file_merge.ipynb) notebook.

## Model Training and Interpretation

This study employed Recurrent Neural Network (RNN)-based models. The training process for the best-performing model, as reported in the paper, is provided in the [`LSTM_train.ipynb`](https://github.com/MinsuChae/MDCRC_Early_Prediction_of_Depressive_Episodes_Seven_Days_BK/blob/main/LSTM_train.ipynb) notebook.  
Model interpretation and feature importance analysis were conducted using SHAP, with the relevant procedures documented in [`LSTM_SHAP.ipynb`](https://github.com/MinsuChae/MDCRC_Early_Prediction_of_Depressive_Episodes_Seven_Days_BK/blob/main/LSTM_SHAP.ipynb).

## Data Availability

Due to IRB restrictions, the dataset cannot be made publicly available or shared with third parties.  
However, the study can be reproduced using data collected through Fitbit devices and patient diagnoses made by qualified medical professionals in accordance with DSM-5 criteria.
