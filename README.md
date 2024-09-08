# Traffic Flow Prediction Project

## Overview
This project aims to develop a predictive model to forecast traffic volume based on various factors such as weather conditions, holidays, and time of day. By leveraging machine learning techniques, the project seeks to provide insights into traffic patterns and improve forecasting accuracy, which can be useful for city planners, transportation authorities, and commuters.

## Dataset
The dataset used for this project contains over 48,000 records of traffic flow and includes the following key features:

- **holiday**: Whether the day is a holiday.
- **temp**: Temperature (in Kelvin).
- **rain_1h**: Amount of rainfall in the past hour (in mm).
- **snow_1h**: Amount of snowfall in the past hour (in mm).
- **clouds_all**: Percentage of cloud coverage.
- **weather_main**: General weather conditions (e.g., Clear, Clouds, Rain).
- **weather_description**: Detailed weather description.
- **date_time**: Timestamp of the record.
- **traffic_volume**: The target variable representing the number of vehicles observed at the station.

## Objectives
The primary goal of the project is to build and evaluate machine learning models that can predict traffic volume based on weather data and other relevant features. Key objectives include:

1. **Data Preprocessing**: Handle missing values, perform feature engineering, and convert categorical variables using one-hot encoding.
2. **Exploratory Data Analysis (EDA)**: Conduct an in-depth analysis to understand relationships between variables, outliers, and trends using visualizations.
3. **Modeling**: Build predictive models using Linear Regression and Random Forest.
4. **Evaluation & Visualization**: Evaluate model performance using metrics such as Mean Squared Error (MSE) and R-squared (R²) and visualize the results.

## Data Preprocessing
- **Handling Missing Data**: Missing values in categorical columns (e.g., holidays) were handled by imputing with the mode.
- **Feature Engineering**: Date and time features were extracted, and irrelevant columns (like date_time) were removed.
- **One-Hot Encoding**: Categorical columns such as holiday, weather_main, and weather_description were converted into numerical values using one-hot encoding.

## Exploratory Data Analysis (EDA)
The EDA provided the following insights:

- Traffic volume shows significant variation based on weather conditions such as rain, cloud coverage, and temperature.
- Holidays tend to have lower traffic volume, indicating fewer people commuting.
- Visualizations such as heatmaps, distribution plots, and pair plots helped uncover the relationships between features.

## Machine Learning Models
Two machine learning models were employed:

- **Linear Regression**: A simple regression model used to establish a baseline prediction of traffic volume.
- **Random Forest**: A more complex ensemble model that captures non-linear relationships between the features and traffic volume.

## Model Performance
- **Linear Regression**:
  - Mean Squared Error (MSE): X.XX
  - R-squared (R²): Y.YY

- **Random Forest**:
  - Mean Squared Error (MSE): X.XX
  - R-squared (R²): Y.YY

The Random Forest model outperformed Linear Regression with a higher R² score, indicating that it captures more variance in the traffic data.

## Visualizations
- **Actual vs. Predicted Traffic Volume**: Line plots were created to visually compare the actual and predicted traffic volumes for both models.
- **Feature Importance**: A bar chart visualizing the most important features in the Random Forest model highlighted weather conditions like temperature and rainfall as significant predictors of traffic flow.
- **Error Distribution**: The error distribution plot for the Random Forest model shows that the majority of the prediction errors are small, indicating good predictive performance.

## Conclusion
This project demonstrated how weather conditions and time-based factors significantly influence traffic volume. The Random Forest model proved to be the most accurate in predicting traffic flow, offering valuable insights for traffic management systems. Future improvements could include using more advanced models or incorporating additional time-series analysis techniques to further refine predictions.

## Technologies Used
- **Python**: For data preprocessing, modeling, and visualization.
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn.
- **Machine Learning Models**: Linear Regression, Random Forest.

## Future Work
- Incorporating real-time data and more advanced time-series forecasting models.
- Exploring deep learning models to further enhance prediction accuracy.
