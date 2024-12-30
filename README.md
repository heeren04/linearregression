# House Price Prediction

This project aims to predict the price of a house based on various features such as location, number of bedrooms, area, and other factors.

## Dataset Overview

The dataset contains 14,620 rows and 22 features that provide details about the house properties. The columns are as follows:

| Column Name                              | Description                                                                 |
|------------------------------------------|-----------------------------------------------------------------------------|
| **ID**                                   | A unique identifier for each house listing (integer)                        |
| **Date**                                 | Date of the listing (integer)                                               |
| **Number of Bedrooms**                   | Number of bedrooms in the house (integer)                                   |
| **Number of Bathrooms**                  | Number of bathrooms in the house (float)                                    |
| **Living Area**                          | Area of the house excluding the basement (integer)                          |
| **Lot Area**                             | Total lot area of the property (integer)                                    |
| **Number of Floors**                     | Number of floors in the house (float)                                       |
| **Waterfront Present**                   | Whether the house is on the waterfront (1 if yes, 0 if no) (integer)        |
| **Number of Views**                      | Number of views the house has (integer)                                     |
| **Condition of the House**               | A rating of the house's condition (integer)                                 |
| **Grade of the House**                   | A grading of the house based on construction quality (integer)              |
| **Area of the House (Excluding Basement)**| Living area excluding the basement (integer)                                |
| **Area of the Basement**                 | Basement area (integer)                                                     |
| **Built Year**                           | The year the house was built (integer)                                      |
| **Renovation Year**                      | The year the house was renovated (integer)                                  |
| **Postal Code**                          | Postal code of the house location (integer)                                 |
| **Latitude**                             | Latitude of the house location (float)                                      |
| **Longitude**                            | Longitude of the house location (float)                                     |
| **Living Area Renovated**                | Renovated living area (integer)                                            |
| **Lot Area Renovated**                   | Renovated lot area (integer)                                               |
| **Number of Schools Nearby**             | Number of schools within a certain radius of the house (integer)            |
| **Distance from the Airport**            | Distance from the house to the nearest airport (integer)                    |
| **Price**                                | The target variable, representing the price of the house (continuous value) |

## Objective

The goal is to create a machine learning model that predicts the **Price** of a house based on the features mentioned above.

## Requirements

To run this project, the following are required:

- Python 3.x
- Libraries:
  - `pandas` for data manipulation
  - `numpy` for numerical operations
  - `scikit-learn` for machine learning algorithms
  - `matplotlib` and `seaborn` for data visualization
  - `xgboost` (optional) for advanced regression models

## Dataset Preprocessing

1. **Handle Missing Data**: If applicable, handle any missing or null values in the dataset.
2. **Feature Engineering**: Extract additional features from existing columns (e.g., extracting the year from the `Date` column).
3. **Feature Scaling**: Normalize or scale features if necessary (e.g., for models sensitive to feature scaling).
4. **Train-Test Split**: Split the dataset into training and testing sets for model evaluation.

## Model Development

1. **Train a Regression Model**: Use machine learning algorithms such as **Linear Regression**, **Random Forest**, or **XGBoost** to predict house prices based on the features.
2. **Model Evaluation**: Evaluate model performance using metrics such as:
   - **R-squared**
   - **Mean Squared Error (MSE)**
   - **Root Mean Squared Error (RMSE)**
3. **Advanced Models**: Consider using **XGBoost** or **Random Forest** for better performance, as they tend to give more accurate results for regression tasks.
