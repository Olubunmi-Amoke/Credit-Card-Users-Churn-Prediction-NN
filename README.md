# Credit-Card-Users-Churn-Prediction Using NN

## Problem Statement
#### Context
Businesses like banks which provide service have to worry about problem of 'Customer Churn' i.e. customers leaving and joining another service provider. It is important to understand which aspects of the service influence a customer's decision in this regard. Management can concentrate efforts on improvement of service, keeping in mind these priorities.
The objective of this project is to build a neural network based classifier that can determine whether a customer will leave the bank or not in the next 6 months.

#### Data Dictionary
CustomerId: Unique ID which is assigned to each customer

Surname: Last name of the customer

CreditScore: It defines the credit history of the customer.

Geography: A customer’s location

Gender: It defines the Gender of the customer

Age: Age of the customer

Tenure: Number of years for which the customer has been with the bank

NumOfProducts: refers to the number of products that a customer has purchased through the bank.

Balance: Account balance

HasCrCard: It is a categorical variable which decides whether the customer has credit card or not.

EstimatedSalary: Estimated salary

isActiveMember: Is is a categorical variable which decides whether the customer is active member of the bank or not ( Active member in the sense, using bank products regularly, making transactions etc )

Exited : whether or not the customer left the bank within six month. It can take two values ** 0=No ( Customer did not leave the bank ) ** 1=Yes ( Customer left the bank )


**Actionable Insights and Business Recommendations**

**Performance Overview**: Handling class imbalance is critical. Models using SMOTE (Synthetic Minority Over-sampling Technique) showed significantly improved recall compared to models without it. Addressing class imbalance in the data via SMOTE played a key role in improving model performance.

**Training vs. Validation Gap**: There are noticeable differences between training and validation recall scores; Among the better performing models, NN model with SMOTE & SGD has the lowest range between the training and validation metric results, indicating reasonable generalization.

**Focus Retention Efforts on Predicted Churners**: Use the best-performing model (e.g., SMOTE + SGD with ~ 0.75 recall on the validation set) to identify high-risk customers and design targeted retention campaigns.

**Improve the model’s utility in identifying churners**: While the current results are promising, aim for recall values above 0.80 on the validation set to minimize false negatives further.
