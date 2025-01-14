# Loan-Approval-Prediction-ML
This project implements a machine learning pipeline to predict loan approval status based on customer attributes. The dataset is preprocessed, balanced, and analyzed using various classification algorithms to achieve reliable predictions. Below is a summary of the key functionalities in the code:

    Data Loading and Exploration:
        The dataset (LoanApprovalPrediction.csv) is loaded using pandas.
        Initial exploration includes displaying the first and last 10 rows, dataset summary (info()), and descriptive statistics (describe()).

    Data Cleaning and Preprocessing:
        The Loan_ID column is dropped as it is not predictive.
        Missing values are handled by imputing the mean for numerical columns and categorical attributes.
        The dataset is balanced using upsampling to address the imbalance in the target variable (Loan_Status).

    Feature Engineering:
        Categorical features (Gender, Married, Education, etc.) are encoded using one-hot encoding.
        Numerical features are standardized using StandardScaler.
        The target variable (Loan_Status) is label-encoded for compatibility with ML models.

    Dataset Splitting:
        The processed dataset is split into training and testing subsets with an 80-20 split ratio.

    Model Training and Evaluation:
        Three machine learning algorithms are used:
            Logistic Regression
            K-Nearest Neighbors (KNN)
            Random Forest Classifier
        Each model is trained on the training data, and predictions are made on the test set.
        Model performance is evaluated using:
            Classification Report: Precision, recall, F1-score
            Accuracy Score

This project provides a foundational pipeline for predictive modeling in the loan approval domain, demonstrating end-to-end machine learning practices.    
