# Diseases_prediction

The project builds a heart disease prediction system using machine learning.

Dataset was acquired from Kaggle and loaded into a Pandas DataFrame.

Data contained attributes like age, sex, chest pain type, cholesterol, ECG results, blood pressure, etc.

Missing values in numeric features (e.g., blood pressure, cholesterol, slope) were filled using mean imputation.

Categorical and boolean features were one-hot encoded for compatibility with ML models.

Exploratory Data Analysis (EDA) was performed using histograms and correlation heatmaps.

Analysis showed strong correlations among certain health indicators.

Target column (num) was simplified to a binary classification:

0 = no heart disease

1 = heart disease present

Dataset was split into training and testing sets using train_test_split.

StandardScaler was applied to normalize numeric features.

Logistic Regression was trained as a baseline model.

Logistic Regression achieved about 84% accuracy.

Performance was evaluated using precision, recall, F1-score, and confusion matrix.

To improve accuracy, a Random Forest classifier was trained.

Random Forest achieved about 88% accuracy, higher than Logistic Regression.

Feature importance analysis identified key predictors such as chest pain type, thalassemia, and slope.

The Random Forest model and scaler were saved using Joblib for future reuse.

A sample CSV template was created for user input (patient health records).

User-uploaded data was preprocessed with the same pipeline (missing value handling, encoding, scaling).

Predictions were made using the saved Random Forest model.

Final results included a new column Heart_Disease_Prediction (0 = no disease, 1 = disease present).

The workflow covers all ML stages: data acquisition, preprocessing, visualization, model training, evaluation, feature interpretation, and deployment.

This makes it a solid foundation for predictive healthcare applications.
