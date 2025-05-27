# Credit Card Fraud Detection

**Author:** Sonia James

---

## Executive Summary

### Rationale

Credit card fraud is a serious and costly problem affecting consumers, businesses, and financial institutions worldwide. Detecting fraudulent transactions early helps prevent significant financial losses, protects customers’ sensitive information, and maintains trust in digital payment systems.

With the increasing volume of online and contactless transactions, fraudsters constantly evolve their tactics, making it critical to have effective, data-driven methods to identify suspicious activity quickly and accurately. Improved fraud detection safeguards both companies and consumers from the negative impacts of fraud, such as monetary loss, legal liabilities, and damaged reputations.

Therefore, studying and improving credit card fraud detection models is essential to enhancing security, reducing fraud-related costs, and ensuring safer financial transactions for everyone.

---

## Research Question

**Can we accurately detect whether a given transaction is fraudulent or not?**

---

## Data Sources

The dataset used for this project is sourced from Kaggle:  
[Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/dntai1983/fraud-data/data)

---

## Methodology

To address the problem of credit card fraud detection, the following methods were used:

- **Data Cleaning and Preparation:**  
  Handling missing values, encoding categorical variables (using target encoding for high-cardinality features and one-hot encoding for low-cardinality features), and scaling numerical features to prepare the dataset for modeling.

- **Exploratory Data Analysis (EDA):**  
  Visualizing key features such as transaction amount, age, time of transaction, and location to understand patterns related to fraudulent behavior.

- **Feature Engineering:**  
  Extracting meaningful features from transaction timestamps (hour, day, weekend flag) and incorporating location data to help the model detect anomalies.

- **Modeling:**  
  Training machine learning classifiers such as **Random Forest** and **Logistic Regression** to predict whether a transaction is fraudulent.

- **Evaluation:**  
  Assessing model performance using metrics including accuracy, precision, recall, and ROC AUC score.

- **Validation:**  
  Splitting the dataset into training and testing sets to evaluate the model’s performance on unseen data and reduce the risk of overfitting.

---

## Results

Key findings from the data analysis include:

- High-value transactions by younger users are more likely to be fraudulent.
- Larger transaction amounts tend to have a slightly higher risk of fraud.
- Fraudulent transactions increase during holiday seasons.
- Fraudulent activities are more common during nighttime hours.

Model performance metrics:

| Model               | ROC AUC Score | Confusion Matrix               |
|---------------------|---------------|-------------------------------|
| Logistic Regression  | 0.916         | `[[62505, 5061], [94, 262]]`  |
| Random Forest       | **0.992**     | `[[67565, 1], [131, 225]]`    |

The **Random Forest** model outperformed Logistic Regression in this case.

---

## Next Steps

- Tune hyperparameters to further improve model accuracy.  
- Explore ensemble models to enhance predictive performance.  
- Address class imbalance and evolving fraud patterns.  


### Outline of project

- https://github.com/sonia-james/AIML_Capstone_part1/blob/main/Fraud_Detection_phase1.ipynb




