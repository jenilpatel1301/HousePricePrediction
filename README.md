# House Price Prediction

# README

This repository contains a Python script for analyzing and predicting housing prices using machine learning techniques. The script utilizes the `numpy`, `pandas`, `matplotlib`, and `seaborn` libraries for data manipulation, visualization, and analysis. The main goal is to demonstrate the process of loading data, preprocessing, exploratory data analysis, feature engineering, and building predictive models.

## Prerequisites

Before running the script, ensure that you have the following dependencies installed:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install these dependencies using pip:

```
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Getting Started

1. Clone this repository to your local machine or download the script directly.

2. Place the `housing.csv` file in the same directory as the script. This file contains the housing data used for analysis and prediction.

3. Run the script using a Python interpreter or in a Jupyter Notebook environment.

## Usage

The script performs the following steps:

1. Imports the necessary libraries: `numpy`, `pandas`, `matplotlib`, and `seaborn`.

2. Loads the housing data from the `housing.csv` file using `pandas` and displays the first few rows of the dataset.

3. Prints the summary information of the dataset, including the number of non-null values and data types of each column.

4. Drops rows with missing values from the dataset using the `dropna` function.

5. Prints the updated summary information of the dataset after removing the missing values.

6. Splits the dataset into input features (`X`) and target variable (`y`) using the `train_test_split` function from `scikit-learn`.

7. Performs exploratory data analysis by visualizing the histograms of the features using `matplotlib`.

8. Creates a correlation heatmap using `seaborn` to visualize the correlations between features.

9. Applies logarithmic transformation to certain features to improve their distribution.

10. Updates the dataset by converting the categorical variable (`ocean_proximity`) into binary dummy variables using `pd.get_dummies`.

11. Creates a correlation heatmap for the updated dataset.

12. Creates a scatter plot to visualize the relationship between latitude, longitude, and median house value.

13. Performs feature engineering by calculating the bedroom ratio and updating the households feature.

14. Splits the updated dataset into test data (`X_test`, `y_test`).

15. Applies the same transformations to the test data as done for the training data.

16. Uses a linear regression model from `scikit-learn` to fit the training data and calculate the score on the test data.

17. Uses a random forest regressor from `scikit-learn` to fit the training data and calculate the score on the test data.

18. Performs a grid search using `GridSearchCV` from `scikit-learn` to find the best hyperparameters for the random forest regressor.

19. Uses the best random forest regressor obtained from the grid search to calculate the score on the test data.

## Results

The script provides insights into the dataset through exploratory data analysis and visualizations. It builds and evaluates two predictive models: linear regression and random forest regression. The performance of the models is assessed using the R-squared score on the test data. The random forest regressor achieved a higher R-squared score compared to linear regression, indicating better predictive performance.

Feel free to modify the script, experiment with different models, and explore further to enhance the analysis and prediction of housing prices.


