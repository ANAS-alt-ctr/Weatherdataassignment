# **Weather assignment**

Weather_assignment.ipynb – Full Python Implementation
Core Libraries & Imports:

NumPy, Pandas for data manipulation

scikit-learn modules: train_test_split, ColumnTransformer, SimpleImputer, OneHotEncoder, MinMaxScaler, Pipeline, SelectKBest, chi2, DecisionTreeClassifier, LinearRegression, LogisticRegression

Data Preprocessing Pipeline:

Loads Weather Data.csv (8,784 hourly records)

Aggregates 50+ raw weather categories to 5 primary classes: Cloudy, Clear, Rain, Snow, Fog (and "other" for infrequent cases)

Encodes reduced categories numerically (0-6 mapping)

Feature Engineering & Transformation:

Imputation: Imputes missing values in specified columns

Scaling: Uses MinMaxScaler to scale features to range​

Column Selection: Treats numerical and categorical variables differently

Uses SelectKBest with chi-squared scoring for feature selection

Models Tested:

DecisionTreeClassifier (main classifier)

LinearRegression

LogisticRegression

Pipeline Structure:
Three-stage pipeline integrating imputation → scaling → Decision Tree classification for weather forecasting.
