
END-TO-END DATA PREPARATION PIPELINE
====================================

1. DATASET INFORMATION
----------------------
Dataset Name: Titanic Dataset
Source: Kaggle
Total Records: 891
Total Features: 10

The dataset contains passenger information
such as age, gender, ticket fare and passenger class.

Target Column: Survived
0 = Did not survive
1 = Survived


2. EDA FINDINGS
---------------
Overall Survival Rate: 38.38%

Survival Rate by Gender:
Sex
female    74.203822
male      18.890815

Survival Rate by Passenger Class:
Pclass
1    62.962963
2    47.282609
3    24.236253

Median Passenger Age: 28.00

The graphs show the survival distribution,
age distribution, fare distribution and
correlation between numerical features.


3. DATA CLEANING
----------------
- Removed duplicate records.
- Replaced invalid age values with missing values.
- Replaced negative fare values with missing values.
- Removed PassengerId, Name, Ticket and Cabin.
- Created FamilySize feature.
- Created IsAlone feature.


4. PREPROCESSING
----------------
Numerical Features:
- Missing values filled using median.
- StandardScaler applied.

Categorical Features:
- Missing values filled using most frequent value.
- OneHotEncoder applied.

Target Column:
- Survived was separated from input features.


5. TRAIN TEST SPLIT
-------------------
Training Data: 80%
Testing Data: 20%

Random State: 42
Stratified splitting was used.


6. OUTPUT FILES
---------------
- clean_dataset.csv
- X_train.csv
- X_test.csv
- y_train.csv
- y_test.csv
- preprocessing_pipeline.joblib
- plots folder


7. CONCLUSION
-------------
The raw Titanic dataset was cleaned and prepared
for machine learning.

Missing values, categorical features and
numerical features were handled using a
preprocessing pipeline.

The final training and testing datasets
are ready for machine learning models.
