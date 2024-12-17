# PHASE-1
Jishnu-E- Phase 1 Capstone Project
#Machine Learning Project: Taiwan Air Quality Index Data#

Project Overview: This project involves analyzing the Taiwan Air Quality Index (AQI) dataset to understand the trends in air quality and identify the relationship between various pollutants such as PM2.5, CO, SO2, and others. The primary goal is to predict the AQI levels based on concentrations of these pollutants using regression analysis techniques. The dataset spans from 2016 to 2024, offering a comprehensive view of Taiwan's air quality over time.

Problem Statement: The project aims to forecast the Air Quality Index (AQI) for various regions in Taiwan and predict pollutant levels, particularly PM2.5, based on historical data. This would assist in improving air quality management and provide insights into the factors affecting air quality. Regression techniques will be employed to model the relationship between AQI and pollutant levels, thereby predicting air quality for future time periods.

Project Objective:
Forecast the Air Quality Index (AQI) based on the levels of specific pollutants.
Predict PM2.5 levels and their impact on air quality.

Data Description:The dataset contains multiple features that represent different aspects of air quality measurements at various monitoring stations across Taiwan. Below is a summary of the dataset’s key features:
Source: https://www.kaggle.com/datasets/taweilo/taiwan-air-quality-data-20162024
Key Features:
 Date: Date and time of the reading (Text)
 Sitename: Name of the monitoring station (Text)
 County: County or city (Text)
 AQI: Air Quality Index (Numeric)
 Pollutant: Main pollutant affecting the air quality (Text)
 Status: Status of air quality (Text)
 Pollutants (SO2, CO, O3, PM10, PM2.5, NO2, NOx, NO): Various air pollutants 
 measured in different units such as ppb, ppm, etc. (Numeric)
 Wind Speed & Direction: Meteorological data for wind (Numeric)
 Average Pollutant Levels: Moving averages for pollutants such as PM2.5, PM10, SO2, 
 CO, etc. (Numeric)
 Geographical Coordinates: Latitude and longitude of the monitoring station 
 (Numeric)
 Station ID: Unique identifier for the station (Numeric)
 
Data Collection: The dataset is imported from Kaggle, which includes a comprehensive set of readings on air quality. The data is gathered from various monitoring stations across Taiwan over the period from 2016 to 2024. The first step in the project is to load and explore the dataset to understand its structure and gain insights into its distribution and relationships.

Data Preprocessing & Cleaning:Handling Missing Values: The dataset is checked for missing values. These are handled through imputation techniques like mean imputation or using more advanced methods such as KNN imputation, depending on the feature’s distribution.

Outlier Detection: Outliers are identified using statistical methods (e.g., Z-scores, IQR). These outliers are either removed or capped to ensure that the model is not skewed by extreme values.

Data Transformation: Numerical features that exhibit skewness are transformed using logarithmic or other methods to normalize their distributions, ensuring better model performance.

Exploratory Data Analysis (EDA): Through EDA, we gain deeper insights into the dataset. Various statistical and visual techniques are applied to understand the 
data better.
Visualizations: The following plots are generated:
Histograms: To visualize the distribution of pollutants and AQI.
Boxplots: To detect outliers in pollutant levels.
Pair Plots: To analyze the relationships between multiple features.
Heatmap Correlation: To identify highly correlated features.
Pie Diagrams: For categorical distributions such as pollutant types.
Bar Plots and Count Plots: To visualize the frequency and distributions of different pollutants.
Line Plots: To analyze the trend of AQI over time.
Kernel Density Estimation (KDE): To analyze the distribution of AQI and pollutants.

Feature Engineering: Encoding Categorical Data: Categorical variables like sitename, county, pollutant, and status are encoded using techniques such as one-hot encoding or label encoding, depending on their cardinality.

Creating New Features: New features such as moving averages for pollutants like PM2.5, PM10, and SO2 are derived to capture trends and fluctuations over time, which can enhance model accuracy.

Feature Selection: Feature Importance: Using models like Random Forest, we assess feature importance to identify which variables most influence the prediction of AQI. This helps in reducing the dimensionality of the data by focusing on the most relevant features.

Select K Best: Statistical tests (such as chi-square) are applied to select the best features for the prediction task. Irrelevant or redundant features are removed to improve model efficiency.

Model Building: Regression algorithms like Linear Regression, Decision Trees, and Random Forest are employed to predict AQI based on the input features.

The best model is selected based on performance metrics such as RMSE (Root Mean Squared Error) or MAE (Mean Absolute Error).

Conclusion: The project aims to create a model that predicts the AQI effectively based on the levels of various pollutants. By analyzing the relationships between air quality and pollutants such as PM2.5, CO, and SO2, the model will help forecast air quality levels and potentially improve environmental policy-making. This can be a valuable tool for government agencies, environmentalists, and the general public to take proactive measures to protect public health.
