Telecom Customer Churn Prediction

Project Overview This project focuses on predicting customer churn for
high-value customers in the telecom industry using a machine learning
model. Customer churn refers to the situation when customers stop using
the service or switch to another provider. Retaining high-value
customers is crucial for a telecom company, and this project aims to
identify potential churners using historical usage data over a
four-month period.

Objective The main goal of this project is to build a predictive model
to: 1. Identify customers at risk of churning. 2. Understand key factors
that lead to churn. 3. Provide actionable insights to the company for
targeted interventions.

Dataset The dataset contains customer-level data over a four-month
period, focusing on high-value customers. Key features include: -
Customer ID: Unique identifier for each customer. - ARPU (Average
Revenue Per User): Measures the revenue generated per user. - Data
Usage: Amount of data used by the customer. - Voice Usage: Call minutes
used by the customer. - Facebook Usage: Social media usage. - Customer
Tenure: How long the customer has been using the service. - Churn:
Whether the customer has churned or not.

Key Steps 1. Data Preprocessing:  - Removal of missing values.  -
Feature engineering to extract key usage metrics.  - Filtering
high-value customers based on usage and revenue thresholds.  - Labeling
churners and non-churners.

2\. Exploratory Data Analysis (EDA):  - Distribution analysis of ARPU,
data usage, and other variables.  - Correlation analysis to understand
relationships between variables and churn.

3\. Model Building:  - Train-Test Split: The data was split into
training and test sets.  - Model Selection: Various models, including
Logistic Regression, Random Forest, and XGBoost, were tested.  - Model
Evaluation: Performance was evaluated using accuracy, precision, recall,
and AUC-ROC scores.

4\. Feature Importance:  - Identified key drivers of churn, such as
ARPU, data usage, and customer tenure.

5\. Model Tuning:  - Hyperparameter tuning was performed to optimize
model performance.

6\. Prediction:  - The final model was used to predict the likelihood of
churn for the test set.

Results - Best Performing Model: Random Forest with an accuracy of X%,
precision of Y%, and recall of Z%. - Top Features Contributing to Churn:
 1. ARPU 2. Data usage 3. Customer tenure - The model successfully
identified customers with a high risk of churning, allowing the company
to target retention strategies effectively.

Visualizations Key visualizations include: - Distribution of ARPU, data
usage, and customer tenure across churners and non-churners. - Feature
importance plot showing the most influential factors contributing to
churn. - Confusion matrix and ROC curve to evaluate model performance.

Conclusion The project successfully built a machine learning model to
predict churn in high-value telecom customers. The results provide
actionable insights for customer retention efforts, allowing the telecom
company to focus on customers most likely to churn and take proactive
steps to retain them.

How to Run the Project 1. Load the Repository: Use the
telecom_churn_data.csv, load the file into google drive and import from
google.colab import drive drive.mount(\'/content/drive\')

df = pd.read_csv(r\"drive/My Drive/Telecom
Project/telecom_churn_data.csv\")

2\. Install the Dependencies: Install the necessary Python libraries and
pip install -r requirements.txt

3\. Run the File in Colab : Open the \`Telecom_Casestudy.ipynb\` file in
Colab and execute the cells to run the analysis and model-building
process.

4\. Visualize the Results: The notebook includes code to generate the
key visualizations used in the analysis.

Dependencies - Python 3.x - Colab - Libraries:  - pandas  - numpy  -
matplotlib  - seaborn  - scikit-learn  - xgboost
