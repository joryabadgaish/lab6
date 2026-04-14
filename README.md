# lab6
# Ecommerce Customers - Linear Regression Lab

## Overview
This project applies **Linear Regression** on the **Ecommerce Customers** dataset to predict **Yearly Amount Spent** based on customer behavior and membership information.

---

## Steps

### 1. Import Libraries
We first import the required Python libraries:
- **pandas** for handling data
- **numpy** for numerical operations
- **matplotlib** and **seaborn** for visualization

### 2. Load the Dataset
The dataset is loaded into a **DataFrame** using `pd.read_csv()` so we can work with it in Python.

### 3. Explore the Data
We use:
- `head()` to view the first rows
- `info()` to check data types and missing values
- `describe()` to see summary statistics
- `columns` to display column names

This helps us understand the dataset before modeling.

### 4. Perform Basic Data Cleaning
We check for missing values using `isnull().sum()`.  
If there are no missing values, no cleaning is needed.

### 5. Exploratory Data Analysis
We create visualizations such as:
- **pairplot** to see relationships between variables
- **heatmap** to view correlation between numeric columns
- **jointplots** to examine how features relate to yearly spending

This helps us understand patterns in the data.

### 6. Prepare the Data for Modeling
We define:
- **X** as the input features:
  - Avg. Session Length
  - Time on App
  - Time on Website
  - Length of Membership
- **y** as the target variable:
  - Yearly Amount Spent

Text columns such as name, email, and address are excluded because the model needs numeric data.

### 7. Split the Data
The dataset is split into:
- **training data** to train the model
- **testing data** to evaluate the model

This is done using `train_test_split()`.

### 8. Train the Model
We use the same model as the lab:
**Linear Regression**

The model is trained using the training data with `.fit()`.

### 9. Make Predictions
After training, the model predicts values for the test data using `.predict()`.

### 10. Evaluate the Model
We evaluate the model using:
- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)

These metrics show how close the predicted values are to the actual values.

### 11. Interpret the Coefficients
The coefficients show how each feature affects **Yearly Amount Spent**.

For example, a larger coefficient means that feature has a stronger effect on customer spending.

---

## Conclusion
The Linear Regression model was successfully applied to the Ecommerce Customers dataset.  
The project followed the same steps as the original lab:
data loading, exploration, cleaning, visualization, model training, prediction, and evaluation.

This lab helps demonstrate how machine learning can be used to predict customer spending behavior.
