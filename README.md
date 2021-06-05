# Credit-Card-Approval-Prediction
**Problem Statment** - A Company wants to automate the Credit Card eligibility process based on customer detail provided while filling online application form & Credit history of the customer.

They have given a problem to identify the customer segments which are eligible for Credit Card approval, so that they can specifically target these customers.

Dataset downloaded from Kaggle - https://www.kaggle.com/rikdifos/credit-card-approval-prediction

Deployed ML Model using Heroku    - https://creditcard-approval-prediction.herokuapp.com/

Deployed ML Model using Streamlit - https://share.streamlit.io/vinaykhujat/credit-card-approval-prediction/main

Visualized data using Tableau - https://public.tableau.com/app/profile/vinay.khujat/viz/CreditCardApprovalPrediction/Dashboard2

# Steps Performed - 
1. Imported both input CSV files using Pandas read_csv function
2. Checked shape of both DataFrames using shape function
3. Checked Null values using isnull function
4. Dropped some columns & duplicated rows, which are not required
5. Checked unique values from Categorical columns using value_counts() function
6. Dropped unnecessary columns using drop function
8. Used Boxplot to check outliers in Numerical columns & removed outliers (if exists)
9. Grouped credit_df on 'ID' column using Groupby function
10. Merged 2 DataFrames using merge function
11. Visualized data using different graphs (Pie, Bar, Histogram, Scatter Plot) using Matplotlib & Seaborn library.
12. Used LabelEncoder to convert Categorical columns to Numerical columns
13. Selected Features & Targeted Column & assigned to a Variable
14. Created Training & Testing Data using train_test_split
15. Used following Classification Machine Learning models & checked Accuracy & Confusion Matrix
    1. Logistic Regression
    2. Decision Tree classification
    3. Random Forest classification
    4. Support Vector Machine classification
    5. K Nearest Neighbor classification
    6. XGBoost  classification
    Accuracy is around 75% , but Precision score is not good, 
17. Normalized the data using MinMax Scalar
18. As data is imbalanced, used imblearn.over_sampling to balance the data
19. Again used all above mentioned ML models & checked Accuracy & Confusion Matrix
    Maximum Accuracy is around 84.14% using XGBoost Model.
21.   Used K-Fold & Stratified Shuffle Split for Validation

**Conclusion** - 
As we have seen that, XGBoost Model is giving the highest accuracy of 84.14 %, hence we will use XGBoost Model for prediction.
