# Tourism Resource Prediction

## Project Overview

This project explores the analysis and prediction of tourism resource allocation using environmental factors and visitor data. The dataset contains information on various environmental factors (such as temperature, air quality, and noise level) and visitor statistics. The goal is to analyze how these factors influence visitor counts and satisfaction, and ultimately, build a predictive model to estimate resource allocation needs for tourism sites.

## Key Features

- Data preprocessing and cleaning
- Exploratory data analysis (EDA) to visualize distributions and correlations
- Feature engineering to categorize environmental factors
- Visualization of environmental factors' influence on visitor satisfaction and visitor count
- Predictive modeling using Linear Regression and Random Forest models

## Dataset

The dataset used in this project contains the following key features:

- **temperature**: Temperature of the tourism site
- **air_quality_index**: Air quality index at the site
- **noise_level**: Noise level at the site
- **visitor_count**: Number of visitors at the site
- **visitor_satisfaction**: Satisfaction rating of visitors
- **timestamp**: Date and time when the data was recorded
- **location_id**: Identifier for the tourism site location
- **season**: The season in which the data was collected
- **resource_allocation**: Allocation of resources at the site (such as staffing and amenities)

## Project Goals

1. **Data Exploration**: Explore the relationships between environmental factors and visitor statistics through visualizations.
2. **Predictive Modeling**: Build predictive models using historical data to forecast resource allocation needs.
3. **Visitor Satisfaction**: Investigate how temperature, air quality, and noise levels affect visitor satisfaction.
4. **Correlation Analysis**: Identify the most significant variables influencing tourism resource allocation.

## Detailed Steps in the Project

### 1. Data Preprocessing:

- Loaded the dataset and checked for missing values.
- Cleaned the dataset by removing rows with missing values.
- Converted the `timestamp` to datetime format.

### 2. Exploratory Data Analysis (EDA):

- Visualized the distribution of environmental factors (temperature, air quality, and noise levels).
- Examined relationships between environmental factors and visitor count.
- Created bar plots for the average visitor count and satisfaction by categorized environmental factors.

### 3. Feature Engineering:

- Created categories for temperature, air quality, and noise level to simplify the analysis and make the data more insightful.

### 4. Predictive Modeling:

- Trained a **Linear Regression** model to predict resource allocation (`resource_prediction`).
- Evaluated the model using Mean Squared Error (MSE) and R-squared metrics.
- Trained a **Random Forest** model for comparison and evaluation.

### 5. Correlation Analysis:

- Generated a heatmap to visualize the correlation between different variables.

## Results

- The **Linear Regression** model achieved:

  - **Mean Squared Error (MSE)**: 0.0104
  - **R-squared (R²)**: 0.6326

- The **Random Forest** model achieved:
  - **Mean Squared Error (MSE)**: 0.0117
  - **R-squared (R²)**: 0.5851

From the results, we can see that the Linear Regression model performed slightly better than the Random Forest model, in terms of both MSE and R² scores. This indicates that the environmental factors in the dataset have a moderate relationship with resource allocation prediction, but there's still room for improvement.

## Future Work

- Explore other machine learning algorithms such as Support Vector Machines (SVM) or Gradient Boosting to improve prediction accuracy.
- Consider incorporating external factors like holiday seasons or special events in the area.
- Use real-time data to create an interactive tool for resource management in tourism sites.

## Acknowledgements

- Dataset: [Tourism Resource Management Dataset - Kaggle](https://www.kaggle.com/datasets/ziya07/tourism-resource-management-dataset)
