# Startup Profit Prediction
# Multiple-Lenior-Regression.
This projects shows a simple implementation of multiple lenior regression.

### Dataset

The dataset consists of the following columns:

- **R&D Spend**: The amount spent on research and development.
- **Administration**: The amount spent on administration.
- **Marketing Spend**: The amount spent on marketing.
- **State**: The state in which the startup is located (New York, California, Florida).
- **Profit**: The target variable, which represents the profit of the startup.

### Steps Taken

1. **Data Loading**: The dataset is loaded using `pandas.read_csv()`.
2. **Feature Selection**: Features (X) are selected by excluding the 'Profit' column, while the target variable (y) is the 'Profit' column.
3. **State Encoding**: The 'State' column is encoded using `pd.get_dummies()` to handle categorical data by converting the states into binary variables.
4. **Data Splitting**: The data is split into training and testing sets using `train_test_split` from `sklearn.model_selection`.
5. **Model Training**: A linear regression model is trained on the training data using `LinearRegression` from `sklearn.linear_model`.
6. **Model Evaluation**: The model's performance is evaluated using the R-squared metric, which measures how well the model explains the variance in the target variable.

### Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `sklearn`: For building and evaluating the machine learning model.

### Results

The R-squared score is used to evaluate the performance of the linear regression model. This score indicates how well the model fits the data, with a score closer to 1.0 being a better fit.
