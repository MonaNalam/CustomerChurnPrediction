# CustomerChurnPrediction
This project aims to predict whether a customer will discontinue a subscription-based service using historical customer data. The model is built using **Decision Tree Classifier** and provides insights into the most significant factors contributing to churn.

# Objective

- Predict whether a customer is likely to churn (i.e., stop using the service).
- Analyze customer behavior based on:
  - Usage patterns
  - Demographic details
  - Subscription tenure
- Handle missing values using appropriate imputation strategies.
- Identify key features that influence customer churn.

# Technologies Used

- Python
- Pandas, NumPy (Data processing)
- Scikit-learn (Modeling, preprocessing, evaluation)
- Matplotlib (Visualization)
- Seaborn (Exploratory analysis)


# Dataset

The dataset used in this project is `Churn_Modelling.csv`, which contains customer data such as:
- Credit Score
- Geography
- Gender
- Age
- Balance
- Number of Products
- Active status
- Estimated Salary
- Churn label (Exited)

---- Columns like `CustomerId`, `RowNumber`, and `Surname` are dropped as they are irrelevant for prediction.

# Workflow

1. **Data Cleaning & Preprocessing**
   - Drop unnecessary columns
   - Handle missing values using `SimpleImputer`
   - Encode categorical variables using `get_dummies`
   - Feature scaling using `StandardScaler`

2. **Model Building**
   - Decision Tree Classifier (`max_depth=3`)
   - Training on 75% of the data, testing on 25%

3. **Model Evaluation**
   - Accuracy, Precision, and Classification Report
   - Visualization of the decision tree

4. **Prediction on New Samples**
   - Input a new customer profile
   - Apply same preprocessing steps
   - Predict churn probability
