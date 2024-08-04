# Customer Churn Metric Dashboard and Prediction Model

## Project Background
Since the cell phone market is now saturated, the huge growth in the wireless market has tapered off. Communications companies are now engaged in battles to attract each other’s customers while retaining their own. Attracting new customers is much more expensive than retaining existing ones, so a good deal of marketing budget is allocated to prevent churn. Therefore it is necessary to know more about customers in advance who is at risk of churning. This project consists of three parts: 
1. Customer Retention Dashboard
2. Classification Model
3. Churn Probability Estimation

## Understanding Dataset
The 'Churn-Dataset' has 7043 rows and 23 columns. 
1. Churn: Customers who left within the last month(as the dataset does not clearly indicate the date, I assume the customer end the contract with company on Jun, 2024)
2. Services each customer has signed up for: phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
3. Customer account information: how long as a customer, contract, payment method, paperless billing, monthly charges, total charges and number of tickets opened in the categories administrative and technical
4. Demographic info about customers – gender, age range, and if they have partners and dependents

## Customer Retention Dashboard

**Overview Page**
[![cstomer-retention1.png](https://i.postimg.cc/nrjM2nPK/cstomer-retention1.png)](https://postimg.cc/Fkv9sXm1)

**Customer Info Page**
[![customer-retention-2.png](https://i.postimg.cc/WzBzfxBB/customer-retention-2.png)](https://postimg.cc/sGJ3MHDm)

**Churn Risk Factors**
[![customer-retention3.png](https://i.postimg.cc/J4XGB4JM/customer-retention3.png)](https://postimg.cc/0b88TvcB)

**North Star Metric and Dimensions in dahboard**
1. Totoal Number of Churned Customers till Now
2. Sum of Revenue Churned till Now
3. Monthly Average Revenue per User(ARPU)
4. Average Monthly Revenue 
5. Percentage of Customer Churn till Now
   

## Classification Model

I use PACE framework to guides the entire machine learning project:

**PLAN**
1. Business Understanding
Company want to predict the likehood of customer churn and help the marketing team target their email campaigns, diminishing customer loss.

2. Model Selection
In this project, I choose Classification model as in the real business context, the marketing team will send the email to the customers that are likely to churn therefore the model only needs to predict whether the customers are likely to churn or not, without necessity to tell the specific risk level. Therefore, this binary classification approach aligns well with the goal of identifying customers who should receive targeted retention emails.

**ANALYZE**
1. Data preprocessing:
* Clean and organize the data
* Handle missing values and outliers
* Encode categorical variables
* Normalize or standardize numerical features
  
2. Feature engineering:
* Remove unnecessary and highly-correlated columns
* Create new features that might be predictive of churn
* Select the most relevant features

**CONSTRCT**
1. Model selection:
* Choose appropriate algorithms (e.g., logistic regression, random forest, gradient boosting)
* Split data into training and testing sets

2. Model training and evaluation:
* Train the selected models on the training data
* Evaluate model performance using metrics like accuracy, precision, recall, and F1-score
* Use cross-validation to ensure robustness

**EXECUTE**
1. Fine-Tuning:
* Address any issues such as overfitting or underfitting that may arise during evaluation.

2. Model deployment:
* Implement the best-performing model in your production environment
* Set up a system to score customers regularly














