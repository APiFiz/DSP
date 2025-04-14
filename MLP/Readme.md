# Bank Marketing Campaign Analysis

## Project Overview
This project is based on a Kaggle dataset and was undertaken as part of the Machine Learning Practices (MLP) course at IIT Madras. The objective is to analyze the direct marketing campaigns of a banking institution. The campaigns were conducted via phone calls, and the goal was to determine whether clients would subscribe to a bank term deposit. Using the provided data, we will identify trends, predict subscription outcomes, and propose strategies to improve marketing effectiveness.

## Dataset Description
The dataset consists of data collected from direct marketing campaigns conducted by the bank. The data includes both the training and test datasets, along with a sample submission file.

### Files
- **train.csv**: Training dataset.
- **test.csv**: Test dataset.
- **sample_submission.csv**: Sample submission file for prediction results.

### Features
#### Input Variables:
1. **Last Contact Date**: Date of the last contact with the client.
2. **Age**: Client's age (numeric).
3. **Job**: Type of job (categorical).
4. **Marital**: Marital status (categorical: "married", "divorced", "single").
5. **Education**: Education level (categorical: "unknown", "secondary", "primary", "tertiary").
6. **Default**: Has credit in default? (binary: "yes", "no").
7. **Balance**: Average yearly balance in euros (numeric).
8. **Housing**: Has a housing loan? (binary: "yes", "no").
9. **Loan**: Has a personal loan? (binary: "yes", "no").
10. **Contact**: Contact communication type (categorical: "unknown", "telephone", "cellular").
11. **Duration**: Last contact duration in seconds (numeric).
12. **Campaign**: Number of contacts performed during this campaign for this client (numeric).
13. **Pdays**: Number of days since the client was last contacted from a previous campaign (numeric; -1 indicates no prior contact).
14. **Previous**: Number of contacts performed before this campaign for this client (numeric).
15. **Poutcome**: Outcome of the previous marketing campaign (categorical: "unknown", "other", "failure", "success").

#### Output Variable (Target):
16. **Target**: Indicates if the client subscribed to a term deposit (binary: "yes", "no").

## Evaluation
Submissions are evaluated using the **F1 score** (macro average) between the predicted classes and the true target variable.

## Submission Format
For each ID in the test set, predict a class ("yes" or "no") for the target variable. The submission file must include a header and follow this format:
```
id,target
1,yes
2,no
...
```

## Goals and Objectives
1. **Understand the Data**: Perform exploratory data analysis (EDA) to uncover trends and insights.
2. **Data Preprocessing**: Clean and prepare the data for model training.
3. **Model Training**: Train machine learning models to predict whether clients will subscribe to term deposits.
4. **Evaluation**: Evaluate the models using the F1 macro score.
5. **Business Insights**: Provide actionable insights and recommendations based on the analysis.

## Steps to Follow
1. **Exploratory Data Analysis (EDA):**
   - Understand the distribution of each feature.
   - Identify correlations between features and the target variable.
   - Visualize key insights using graphs and charts.

2. **Data Preprocessing:**
   - Handle missing values in features like `education` and `contact`.
   - Encode categorical variables.
   - Scale numerical features if required.
   - Split the data into training and validation sets.

3. **Model Training and Evaluation:**
   - Train classification models such as Logistic Regression, Random Forest, and XGBoost.
   - Use cross-validation to tune hyperparameters.
   - Evaluate models on the validation set using F1 macro score.

4. **Predictions and Submission:**
   - Generate predictions on the test set.
   - Format the predictions as per the submission guidelines.
   - Submit the results for evaluation.

5. **Insights and Recommendations:**
   - Analyze feature importance.
   - Provide actionable insights to improve campaign success rates.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
- **Platform:** Jupyter Notebook or any Python IDE

## Deliverables
1. Code files for data analysis, preprocessing, and model training.
2. A detailed report explaining the methodology, findings, and recommendations.
3. Final submission file in the required format.
