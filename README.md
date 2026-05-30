# Housing Sales Analysis and Price Prediction

## Project Overview

This project presents a complete end-to-end data analytics and machine learning workflow for housing sales data. The objective was to analyze factors affecting house prices, generate business insights through data visualization, and develop a predictive model capable of estimating housing sale prices.

The project combines data cleaning, exploratory data analysis (EDA), feature engineering, dimensionality reduction, machine learning, and interactive dashboard development using Power BI.

## Dataset

The dataset contains information about residential properties, including location, property size, number of rooms, building type, quality scores, utility availability, registration fees, commission fees, and final sales prices.

The target variable is:

**SALES_PRICE**

## Data Cleaning and Preprocessing

Several preprocessing steps were performed to improve data quality and ensure reliable analysis:

* Removed records with missing bedroom and bathroom information.
* Filled missing values in the overall quality score using mean imputation.
* Removed inconsistencies and spelling errors in categorical columns such as Area, Build Type, Street Type, Utility Availability, Sale Condition, and Parking Facility.
* Converted sale and construction dates into datetime format.
* Identified potential outliers using boxplot analysis.
* Created additional time-based features from sales dates.

A cleaned version of the dataset was exported for use in Power BI dashboard development.

## Exploratory Data Analysis

Exploratory analysis was conducted to understand housing market behavior and identify key factors influencing property prices.

Key analyses included:

* Average sales price by area.
* Top-performing residential locations.
* Housing sales trends over time.
* Distribution of numerical features.
* Outlier detection using boxplots.
* Relationships between property characteristics and sales prices.

## Feature Engineering

Categorical variables were transformed into numerical representations using:

* Label Encoding for Area, Street, Zone, and Building Type.
* One-Hot Encoding for Parking Facility.
* Custom ordinal encoding for Utility Availability and Sale Conditions.

Numerical features such as registration fees and commission fees were standardized using StandardScaler to improve model performance.

## Dimensionality Reduction

Principal Component Analysis (PCA) was applied to reduce feature dimensionality while retaining most of the dataset's information. Based on cumulative explained variance analysis, six principal components were selected for model training.

## Machine Learning Models

Multiple regression algorithms were trained and evaluated to predict housing sales prices:

* Linear Regression
* K-Nearest Neighbors Regressor
* Decision Tree Regressor
* Random Forest Regressor
* XGBoost Regressor

Models were compared using the following evaluation metrics:

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)

## Model Optimization

Hyperparameter tuning was performed using GridSearchCV on the Random Forest Regressor to identify the optimal configuration and improve prediction accuracy.

The final model was trained using the best-performing parameters and achieved the highest predictive performance among all tested algorithms.

## Power BI Dashboard

An interactive Power BI dashboard was developed using the cleaned dataset to provide business insights and support decision-making.

The dashboard includes:

* Sales Overview
* Average Price by Area
* Sales Trend Analysis
* Property Distribution by Building Type
* Key Performance Indicators (KPIs)
* Interactive Filters and Visualizations

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* Jupyter Notebook
* Power BI

## Project Workflow

Raw Dataset → Data Cleaning → Exploratory Data Analysis → Feature Engineering → Data Scaling → PCA → Model Training → Hyperparameter Tuning → Prediction → Power BI Dashboard

## Key Outcomes

* Improved data quality through comprehensive preprocessing.
* Identified important factors affecting housing prices.
* Developed and compared multiple machine learning regression models.
* Optimized model performance using GridSearchCV.
* Built an interactive Power BI dashboard for business reporting and decision support.
* Created a complete data analytics and machine learning pipeline from raw data to actionable insights.

## Author

Kareem Bakr

Computer and Systems Engineering Student | Data Analyst | Front-End Developer

This project demonstrates practical experience in data analysis, machine learning, data visualization, and business intelligence using real-world housing sales data.
