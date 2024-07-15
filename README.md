# Medical-insurance-price-predictor
This project predicts medical insurance prices using the RandomForestRegressor and XG Boost Regressor from scikit-learn. It involves loading the dataset, encoding categorical variables, training the model, and comparing its performance with mean absolute error calculated from both the models
Steps Involved
Data Collection:
The dataset is loaded from a CSV file named insurance.csv. This dataset typically includes features such as age, sex, BMI, number of children, smoking status, region, and the target variable, charges, which represents the insurance price.
Data Preprocessing:

Encoding Categorical Variables: 
The dataset may contain categorical variables (e.g., sex, smoker, region). These are encoded into numerical values using LabelEncoder from scikit-learn.

Feature and Target Separation: 
The features (independent variables) are separated from the target variable (dependent variable). Here, X represents the features and y represents the target variable, charges.

Data Splitting:
The dataset is split into training and testing sets using train_test_split from scikit-learn. Typically, 80% of the data is used for training the model, and 20% is reserved for testing. The random state is set to ensure reproducibility.

Model Training:
A RandomForestRegressor is initialized with 100 trees (n_estimators=100) and a specified random state for reproducibility.
The model is then trained (fitted) on the training data (X_train and y_train).
XG Boost Regressor is used with 100 estimators, learning rate of 0.1  and a specified random state for reproducibility.
The model is then trained (fitted) on the training data (X_train and y_train).

Model Prediction:
The trained model are used to make predictions on the test data (X_test).

Model Evaluation:
The performance of the model is evaluated using the Mean Absolute Error (MAE)
Mean Absolute Error for RandomForestRegressor is 2533.674643617756
Mean Absolute Error for XG Boost Regressor is 2445.7743748322937

Observation:
XG Boost Regressor performs better
