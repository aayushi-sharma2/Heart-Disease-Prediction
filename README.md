# Heart-Disease-Prediction
Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Four out of 5CVD deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age. Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease.

People with cardiovascular disease or who are at high cardiovascular risk (due to the presence of one or more risk factors such as hypertension, diabetes, hyperlipidaemia or already established disease) need early detection and management wherein a machine learning model can be of great help.

# Attributes: 

Age: age of the patient [years]

Sex: sex of the patient [M: Male, F: Female]

ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]

RestingBP: resting blood pressure [mm Hg]

Cholesterol: serum cholesterol [mm/dl]

FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]

RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]

MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]

ExerciseAngina: exercise-induced angina [Y: Yes, N: No]

Oldpeak: oldpeak = ST [Numeric value measured in depression]

ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]

HeartDisease: output class [1: heart disease, 0: Normal]

# Process used for prediction-

Extrapolatory analysis

Data cleaning and Outliers removal

Feature scaling , Train-test split etc to prepare the data for model fitting.

Fitting the training data, prediciting it, making the confusion matrix and calculating the accuracy score.

Comparing accuracy scores for various models.

We first applied various methods for outliers removal: Z value score, IQR method and also fixing range by our understanding.

# Before Z- value standardization and Outliers removal

Logistic Regression: 84.05%
KNN: 71.37%
Logistic Regression with feature scaling: 82.60%
Gaussian Naive Bayes: 84.78%
SVM-svc: 85.21%
SVM- LinearSvc: 82.60%
SVM- NUsvc: 85.21%
Decision Tree: 80.86%
Random Forest Classifier: 87.82%
GBM classifier: 86.7%
GBM regressor: 4%

# After Z- value standardization and Outliers removal

Logistic Regression: 89.51%
KNN: 67.79% (n=7)
Logistic Regression with feature scaling: 87.44%
Gaussian Naive Bayes: 87.89%
SVM-svc: 90.13%
SVM- LinearSvc: 87.44%
SVM- NUsvc: 88.79%
Decision Tree: 78.02%
Random Forest Classifier: 88.34%
GBM classifier: 87%
GBM regressor: 27%

# Best results are from Logistic Regression: 89.51% accuracy & SVM-svc: 90.13% accuracy
