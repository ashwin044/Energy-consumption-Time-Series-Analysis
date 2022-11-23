# Analytical Vidhya Jobathon (November)

#### ***Problem Statement in Brief*** : 
Given the data of Enery consumption of past 10 years, forecast the Energy required for the next 3 years.

#### ***Exploratory Data Analysis (EDA) and Data Pre Processing*** :
* First Step is to Find Missing Values in data (There are 1200 data missing values in energy columns in the dataset)
* Replacing the missing values in the column by pandas fillna() and rolling mean

#### ***Approach***:
* Split 10 yrs Data into ***Training Data (8yrs)*** and ***Testing data (2yrs)***
* Used ***Facebook Prophat model***
* Trained the Facebook Prophat model using the Training Data and predicted the next 2 yrs data
* Calculated ***RMSE*** using the new predicted value with the Actual value (test data )
* Performed ***Hyper Parameter Tunning*** improved model accuracy by changing hyper parameters and reducing RMSE
* Used Best Parameters to predict the future value
