# ML_Prediction_of_political_trust_Python
Classification project - predicting the level of trust in politicians


## Datasets

Source: European Social Survey (ESS)
Link: https://ess.sikt.no/en/

The size of the datasets is too large for both Moodle and GitHub, therefore we made it available for downloading on Google Drive.
Download it here: https://drive.google.com/drive/folders/1FY-zySFCDLBAn1MUeTkgcKyk7X0SQQb6?usp=sharing
After downloading, copy files into: Classification project/data/
The data folder contains 17 CSV and 17 SPSS files corresponding to 11 ESS rounds. In our project, CSV files are treated as source datasets while SPSS files are used to extract variable and value metadata.
Target variable: trstplt  (trust in politicians)

## Objective
The objective of the classification project is to examine what individual characteristics and social factors are the strongest predictors of trust in politicians and to evaluate the predictive performance of different tree-based classification models.

## Models used

- Decision tree classifier
- Random forest classifier
- Gradient boosting classifier

Model parameter tuning was performed using cross-validated grid search for the decision tree and cross-validated randomized search for the ensemble models on a stratified training subsample. The selected models were then refit on the full training set and evaluated on a held-out test set using balanced accuracy as the primary metric, with accuracy, precision, recall, and F1-score reported as secondary metrics.

Jupyter Notebooks (.ipynb) and PDF files contain full code, preprocessing, model tuning, and evaluation.
Presentation PDFs contain 7-10 slides summarizing the project.

## Technical details

Programming language: Python
Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, pyreadstat, IPython, pathlib
All models are implemented using pipelines with preprocessing and missing value imputation.
