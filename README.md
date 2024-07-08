# House Price Prediction Project

This project aims to predict house prices using various machine learning models. The dataset used is `housing.csv`. Below is a summary of the steps followed and models used.

## Libraries Used

- numpy: Provides support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays.
- pandas: Offers data structures and data analysis tools for manipulating numerical tables and time series.
- matplotlib: A plotting library for creating static, interactive, and animated visualizations in Python.
- seaborn: Based on matplotlib, it provides a high-level interface for drawing attractive and informative statistical graphics.
- sklearn (scikit-learn): A machine learning library that provides simple and efficient tools for data mining and data analysis.


## Process Overview

### Data Preprocessing

- **Data Loading and Exploration**
  - Loaded dataset using pandas.
  - Displayed the first and last few rows.
  - Generated a summary using `data.info()`.

- **Categorizing a Numerical Attribute**
  - Categorized `median_income` for stratified splitting.

- **Custom Train-Test Split**
  - Implemented a custom train-test split function.
  - Applied the custom split to the dataset.

- **Stratified Splitting using sklearn**
  - Utilized `StratifiedShuffleSplit` for accurate train-test splits.

- **Handling Categorical Features**
  - One-hot encoded categorical data using both pandas and sklearn.

- **Handling Missing Values**
  - Identified and filled missing values using the median.

- **Feature Scaling**
  - Applied Min-Max scaling.
  - Applied Standard scaling.

### Data Visualization

- **Histograms for All Columns**
  - Visualized distributions of each column using histograms.

- **Correlation Analysis**
  - Computed correlation matrix.
  - Examined correlations with `median_income`.

### Modeling

- **Linear Regression**
  - Trained a linear regression model.
  - Visualized predictions.

- **Decision Tree**
  - Trained a decision tree regressor.
  - Visualized predictions.
  - Conducted cross-validation.

- **Random Forest**
  - Trained a random forest regressor.
  - Conducted cross-validation.
  - Used `RandomizedSearchCV` for hyperparameter tuning.

### Final Steps

- **Final Model**
  - Saved the final model using the Joblib library.

---
