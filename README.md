### Credit card fraud detection

**Sonia James**

#### Executive summary

#### Rationale
Why should anyone care about this question?
Credit card fraud is a serious and costly problem affecting consumers, businesses, and financial institutions worldwide. Detecting fraudulent transactions early helps prevent significant financial losses, protects customers’ sensitive information, and maintains trust in digital payment systems.

With the increasing volume of online and contactless transactions, fraudsters constantly evolve their tactics, making it critical to have effective, data-driven methods to identify suspicious activity quickly and accurately. Improved fraud detection safeguards both companies and consumers from the negative impacts of fraud, such as monetary loss, legal liabilities, and damaged reputations.

Therefore, studying and improving credit card fraud detection models is essential to enhancing security, reducing fraud-related costs, and ensuring safer financial transactions for everyone.

#### Research Question
What are you trying to answer?
I am trying to detect if a given transaction would be fraudulent or not. 

#### Data Sources
What data will you use to answer you question?
Dat from kaggle : https://www.kaggle.com/datasets/dntai1983/fraud-data/data

#### Methodology
What methods are you using to answer the question?
Methods Used
To address the problem of credit card fraud detection, I’m using a combination of data preprocessing, feature engineering, and machine learning models:

Data Cleaning and Preparation:
Handling missing values, encoding categorical variables (using target encoding and one-hot encoding depending on cardinality), and scaling numerical features to prepare the dataset for modeling.
Exploratory Data Analysis (EDA):
Visualizing key features such as transaction amount, age, time of transaction, and location to understand patterns related to fraudulent behavior.
Feature Engineering:
Extracting meaningful features from transaction timestamps (like hour, day, and weekend flag) and using location data to help the model detect anomalies.
Modeling:
Training machine learning classifiers such as Random Forest and Logistic Regression to predict whether a transaction is fraudulent.
Evaluating models using metrics like accuracy, precision, recall, and ROC AUC to understand their effectiveness.
Validation:
Splitting the dataset into training and testing sets to validate model performance on unseen data, reducing the risk of overfitting.

#### Results
What did your research find?
I see below trends from my data analysis : 
---High-value transactions by younger users are more likely to be fraudulent.
---Higher amount also seems to be a little more plone to fraudulant transactions.
---Holiday season has more fraudulant transactions.
---Its also observed that fraudulant transaction occur more in night time.

I used Logistic Regression and Random Forest to create a model. I could get better scores with Random Forest
Logistic regression : 
ROC AUC Score: 0.9164710610050197
Confusion Matrix:
 [[62505  5061]
 [   94   262]]

 Random Forest : 
 ROC AUC Score: 0.9917311396231133
 Confusion Matrix:
 [[67565     1]
 [  131   225]]


#### Next steps
What suggestions do you have for next steps?
Fraud detection is inherently difficult due to imbalanced classes (fraud cases are rare), evolving fraud tactics, and the need for real-time detection.
I want to tune the hyper parameters and use ensemble model to see if i can create a better model 

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
