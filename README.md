#  Customer Churn Prediction ML Model
This project implements a Machine Learning model that predicts whether a customer is likely to **churn (leave the company)** or **stay**, based on their demographic and service-related data. The model is trained using customer data from a telecommunications service provider and aims to help businesses proactively reduce customer attrition.

## Features Used
The model takes into consideration the following input features:

1. Gender  
2. Senior Citizen Status (0: No, 1: Yes)  
3. Partner Status (Yes/No)  
4. Dependent Status (Yes/No)  
5. Tenure (Number of months the customer has stayed)  
6. Phone Service (Yes/No)  
7. Multiple Lines (Yes, No, No phone service)  
8. Internet Service (DSL, Fiber optic, No)  
9. Online Security (Yes/No/No internet service)  
10. Online Backup (Yes/No/No internet service)  
11. Device Protection (Yes/No/No internet service)  
12. Tech Support (Yes/No/No internet service)  
13. Streaming TV (Yes/No/No internet service)  
14. Streaming Movies (Yes/No/No internet service)  
15. Contract Type (Month-to-month, One year, Two year)  
16. Paperless Billing (Yes/No)  
17. Payment Method (Electronic check, Mailed check, etc.)  
18. Monthly Charges  
19. Total Charges  

All categorical columns are encoded using pre-fitted encoders saved in a `.pkl` file.

##  How to Use

To use the model and make predictions on customer data:

1. Clone or download this repository.
2. Ensure the following files are in the same directory:
    - `customer_churn_model.pkl` (Trained ML model)
    - `encoders.pkl` (Dictionary of LabelEncoders for categorical columns)
    - `Customer_churn_prediction.ipynb` (Notebook for prediction)

3. Load the model and encoders using `pickle`.
4. Prepare your input data as a pandas DataFrame matching the model's training format.
5. Use the encoders to transform categorical fields.
6. Use the loaded model to make predictions and get probabilities.
