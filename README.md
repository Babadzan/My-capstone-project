# My-capstone-project
PROJECT TITLE-ONLINE PAYMENT FRAUD DETECTION FOR BLOSSOM BANK PLC

INTRODUCTION:

The introduction of online payment systems has helped a lot in the ease of payments. But, at the same time, it increased in payment frauds. Online payment frauds can happen with anyone using any payment system. That is why detecting online payment fraud is very important for finacial institutions to ensure that the customers are not getting charged for the products and services they never paid. This project looks to build  machine learning models using the dataset of transactions of Blossom bank Plc.

To identify online payment fraud with machine learning, we need to train a machine learning model for classifying fraudulent and non-fraudulent payments. For this, we need a dataset containing information about online payment fraud, so that we can understand what type of transactions lead to fraud. For this task, I made use of the given dataset, which contains historical information about fraudulent transactions from Blossom Bank plc.which can be used to detect fraud in online payments.

DATA DICTIONARY (Description of the Columns):

• step: represents a unit of time where 1 step equals 1 hour

• type: type of online transaction

• amount: the amount of the transaction

• nameOrig: customer starting the transaction

• oldbalanceOrg: balance before the transaction

• newbalanceOrig: balance after the transaction

• nameDest: recipient of the transaction

• oldbalanceDest: initial balance of recipient before the transaction

• newbalanceDest: the new balance of the recipient after the transaction

• isFraud: fraud transaction

STEPS TAKEN:

Importation of necessary Libraries

Data Inspection

Loaded the csv data using pd.read_csv

check rows and columns for better understanding of the data set

Checked the data info to know the total number of columns and the data type of each column

Data Cleansing

Checking  for missing values

Exploratory Data Analysis

Visualized relationships between the label and some key features

Conducted univariate and multivariate analysis using appropraite visualization tools.

# Feature Engineering
Drop unneccesary columns

Conversion of categorical data in Column 'type' to numerical data using One-Hot Encoding (pd.get_dummies())

joining the encoded variables back to the main dataframe using pd.concat()

removing the initial categorical column after it has been encoded 

# Modelling
Selection of features(X) and target(y)

Importation and initialization of necessary libraries for modelling

The ML models used are Random Forest Classifier, KNeighbors, Naive Bayes Classifier and Decision Tree Classifier

# Model evaluation

# Conclution
RandomForest classsifier shows the highest accuracy and precision, hence it can be considered best suited for predicting online payment fraud for Blossom bank plc.
