Loan Amount Prediction: A Comparative Analysis of Regression Models
A machine learning project that predicts the eligible loan amount for an applicant by comparing two different regression algorithms: Linear Regression and Support Vector Regression (SVR).

Overview 📝
This project aims to solve a common business problem for financial institutions: determining the loan amount that can be safely offered to an applicant. By analyzing features such as applicant income, co-applicant income, and credit history, two models are built and evaluated to provide an estimated loan amount.

The process involves:

Data Preprocessing: Cleaning the data, handling missing values, and treating outliers.

Model Training: Implementing and training both a Linear Regression and a Support Vector Regression (SVR) model using Scikit-learn pipelines.

Hyperparameter Tuning: Using GridSearchCV to find the best parameters for the SVR model.

Evaluation & Comparison: Assessing the accuracy of both models using the R-squared metric to determine the best-performing algorithm for this dataset.

Dataset 📁
The dataset used for this project is sourced from a common Kaggle competition. It contains various attributes of loan applicants.The datasets are inlcuded in this repository as train.csv and test.csv

Key Features: ApplicantIncome, CoapplicantIncome, Loan_Amount_Term, Credit_History, Property_Area, etc.

Target Variable: LoanAmount

Installation ⚙️
To run this project locally, follow these steps:

Install the required libraries listed in requirements.txt.

Run the loan.ipynb file present in the repository.

Models & Performance 📊
The performance of both models was evaluated on the held-out test set. The primary metric used for comparison is the R-squared (R²) score, which represents the proportion of variance in the target variable that the model can explain.

Linear Regression
R-squared Score: 0.630

This indicates that the Linear Regression model can explain approximately 63% of the variance in the LoanAmount.

Support Vector Regression (SVR)
R-squared Score: 0.442

After hyperparameter tuning with GridSearchCV, the best SVR model explains approximately 44.2% of the variance in the LoanAmount.

Conclusion
For this specific dataset, the Linear Regression model performed significantly better than the Support Vector Regression model, providing a more accurate prediction of the eligible loan amount.
