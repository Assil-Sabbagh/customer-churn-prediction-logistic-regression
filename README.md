# Customer Churn Prediction Using Logistic Regression

This project predicts whether a telecom customer is likely to leave the company or stay. It uses customer information such as contract type, tenure, monthly charges, total charges, internet service, and payment method to classify customers into two categories: **Churn** and **No Churn**.

The project was developed as an Intro to AI Lab project using a Logistic Regression model. The data was cleaned, prepared, encoded, scaled, and then divided into training and testing sets. The model was trained using gradient descent and evaluated using accuracy, a confusion matrix, and a classification report.

## Project Goal

The goal of this project is to help telecom companies identify customers who may leave early, so they can take action to improve customer retention.

## Dataset

The dataset contains telecom customer information, including:

* Gender
* Senior Citizen status
* Partner and dependents
* Tenure
* Phone service
* Internet service
* Contract type
* Payment method
* Monthly charges
* Total charges
* Churn status

The target column is **Churn**, where:

* `1` means the customer churned
* `0` means the customer did not churn

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Data Cleaning and Preparation

The dataset was prepared using the following steps:

* Removed the `customerID` column because it does not help in prediction.
* Converted `TotalCharges` from text to numeric values.
* Replaced missing values in `TotalCharges` with the median value.
* Converted the target column `Churn` into numbers.
* Encoded categorical columns using `LabelEncoder`.
* Split the dataset into 80% training data and 20% testing data.
* Standardized the features using `StandardScaler`.

## Model

The project uses Logistic Regression built from the main algorithm steps:

* Initialize parameters `w` and `b`
* Apply the sigmoid function
* Perform forward propagation
* Calculate the cost
* Perform backward propagation
* Update parameters using gradient descent
* Predict churn or no churn based on probability

## Results

The model achieved:

* Training Accuracy: **79.46%**
* Testing Accuracy: **80.91%**

Further analysis showed that learning rate `0.01` gave the best result:

* Training Accuracy: **79.78%**
* Testing Accuracy: **80.98%**

## Graphs and Evaluation

The project includes:

* Cost curve
* Churn distribution graph
* Sigmoid function visualization
* Learning rate comparison
* Confusion matrix
* Classification report

## Conclusion

This project shows how Logistic Regression can be used to predict customer churn using telecom customer data. The model achieved good testing accuracy of about 81%, which means machine learning can help companies detect at-risk customers and improve customer retention.

## Contributors

*  Assil Sabbagh
* Cynthia Issa

