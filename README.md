# Heart Attack Analysis & Prediction Using Machine Learning
# Overview
This project involves analyzing heart attack datasets and building predictive models using machine learning techniques. It aims to provide insights into key factors influencing heart disease and to classify patients as being at risk or not using various machine learning algorithms.

# Dataset
The dataset used for this project is publicly available and contains 14 features related to heart health. Key attributes include age, sex, cholesterol levels, maximum heart rate, and others, along with the target variable output (1 = Presence of heart disease, 0 = Absence of heart disease).

# Key Features
1. Age: Patient's age.
2. Sex: Gender of the patient (1 = Male, 0 = Female).
3. 3.cp (Chest Pain Type):
   3.1: Typical angina
   3.2: Atypical angina
   3.3: Non-anginal pain
   3.4: Asymptomatic
5. trtbps: Resting blood pressure (mm Hg).
6. chol: Serum cholesterol (mg/dl).
7. fbs: Fasting blood sugar > 120 mg/dl (1 = True, 0 = False).
8. restecg: Resting electrocardiographic results.
9. thalachh: Maximum heart rate achieved.
10. exang: Exercise-induced angina (1 = Yes, 0 = No).
11. oldpeak: ST depression induced by exercise relative to rest.
12. slp: Slope of the peak exercise ST segment.
13. ca: Number of major vessels colored by fluoroscopy.
14. thal: Thalassemia (1 = Normal, 2 = Fixed defect, 3 = Reversible defect).
15. output: Target variable (1 = At risk of heart disease, 0 = Not at risk).
# Data Analysis and Visualizations
Exploratory Data Analysis (EDA)
1. Null Values: The dataset was checked for missing values, and none were found.
2. Summary Statistics: Statistical summaries provided insights into feature distributions.
Key Observations
1. ST Depression (Oldpeak):
   Patients with heart disease exhibited lower average ST depression (1/3rd of negative patients).
2. Maximum Heart Rate (Thalach):
   Positive patients exhibited a higher average maximum heart rate.
3. Output Distribution:
   Visualized using a pie chart, showing the proportion of patients with and without heart disease.
4. Gender Distribution:
   Gender breakdown revealed a higher prevalence of males in the dataset.
 *Correlation Analysis*
   A correlation heatmap highlighted:
6. Positive correlation between chest pain type (cp) and heart disease.
   Negative correlation between exercise-induced angina (exang) and heart disease.
7. Feature Distributions
   KDE plots were used to visualize the distribution of features like:
8. Age
Cholesterol (Chol)
Maximum Heart Rate (Thalachh)
Resting Blood Pressure (Trtbps)
# Machine Learning Models
Data Preprocessing
Splitting the dataset into training (80%) and testing (20%) sets.
Standardizing features using StandardScaler to normalize data.
Models Implemented
Logistic Regression:
Simplicity and interpretability make it a good baseline model.
Achieved accuracy: 75%
Random Forest Classifier:
A robust ensemble learning method, particularly effective for tabular data.
Achieved accuracy: 80%
Support Vector Machine (SVM):
Kernel trick employed for nonlinear classification.
Achieved accuracy: 77%
# Model Evaluation
Each model was evaluated using:
Classification Report:
Provided precision, recall, F1-score, and support for each class.
Confusion Matrix:
Visualized the model's performance for positive and negative cases.
Accuracy Score:
Overall model performance metric.
# Summary of Results
Model	Accuracy
Logistic Regression	75%
Random Forest 80%
SVM	77%
# Conclusion
This project demonstrates the use of machine learning for predicting heart attack risk based on patient data. Random Forest emerged as the most accurate model, showcasing its capability to handle complex data relationships.
