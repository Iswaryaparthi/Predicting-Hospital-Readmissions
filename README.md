## Predicting Hospital Readmissions

### Objective:

The primary goal of this project is to build a predictive model that can identify patients who are at high risk of hospital readmission within 30 days after their initial discharge.

#### Tasks carried out in this project:

- Importing libraries
- Data Collection and Preprocessing
- Feature Engineering
- Model Building
- Model Evaluation
- Visualizations
- Challenges
- Results and Insights

#### Libraraies to Import:

- import pandas as pd
- import numpy as np
- import seaborn as sns
- import matplotlib.pyplot as plt
- from sklearn.preprocessing import LabelEncoder
- from sklearn.model_selection import train_test_split
- from sklearn.preprocessing import StandardScaler
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.linear_model import LogisticRegression
- from sklearn.metrics import confusion_matrix, accuracy_score, classification_report

#### Data Collection and Preprocessing:

- Check the data for null values, dupliactes, distribution of the data
- Get the statistics of the data
- The given data is a mixture of categorical and continuous
- Convert the categorical data into numeric data using encoders like label, ordinal, one-hot encoders
- Fill the A1C_result column null values by model building

#### Feature Engineering:

- Select the features which is going to help to create model building
- Fill the null values using model building
- Readmitted as target column and others are  independent variable
- Chi Square and ANOVA are used to find the high correlated features
- Age column have outliers and filled with mean values
- Scaling done for the selected features
  
#### Visualizations:

- Build correlation matrix using  heatmap to find the correlation of the variables with target variable
- Histogram, Box plot, Countplot are used to get the distribution of the individual features
- Boxplot, Barplot to get the realtionship among feature and target variable

#### Model Building & Model Evaluation:

- After feature engineering and visualizations will get the idea to select the X and y variable to do model building
- Used Logistic regression, Random tree Classifier, Gradient Boosting for model building
- Selected features are X variable and y as Readmitted column 
- Accuracy score ranged from 0.55%
- Did hyperparameter tuning, GridSearch CV approach are used to best model fit

#### Challenges:
- No data regarding patient admission date or discharge date
- Outliers detected in Age column
- 50% null value present in A1C_result column
- Low accuracy score determined

#### Results and Insights:

- Tried the predicted model with sample data
- Got the result as 47% patients are expecting to readmitted again 
- Age,Num_Medications, Number of diagnoses provided the more information regarding readmission status
- Among 1000 data, around 285 patients are abnormal and will not readmitted and 270 are abnormal and readmitted again

#### Thank you All!

