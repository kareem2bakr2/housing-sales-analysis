Housing Sales Analysis and Price Prediction
Project Overview

This project analyzes housing sales data to uncover factors affecting property prices and builds machine learning models to predict housing sale prices.

The project includes:

Data Cleaning and Preprocessing
Exploratory Data Analysis (EDA)
Interactive Power BI Dashboard
Feature Engineering
Principal Component Analysis (PCA)
Regression Modeling
Hyperparameter Optimization using GridSearchCV
Dataset Information

The dataset contains housing sales information including:

Feature	Description
AREA	Property Area
INT_SQFT	Interior Square Feet
N_BEDROOM	Number of Bedrooms
N_BATHROOM	Number of Bathrooms
N_ROOM	Total Rooms
DIST_MAINROAD	Distance from Main Road
PARK_FACIL	Parking Availability
BUILDTYPE	Building Type
SALES_PRICE	Target Variable

Target Variable:

SALES_PRICE

Data Cleaning

The following preprocessing steps were performed:

Removed missing values from:
N_BEDROOM
N_BATHROOM
Filled missing values in:
QS_OVERALL (Mean Imputation)
Corrected inconsistent categorical values:

Examples:

Column	Correction
Noo → No	PARK_FACIL
Comercial → Commercial	BUILDTYPE
Chormpet → Chrompet	AREA
Pavd → Paved	STREET
Converted date columns to datetime format.
Exploratory Data Analysis

Key analyses performed:

Average Housing Price by Area

Identified the top-performing residential areas based on average sales price.

Yearly Sales Trend

Analyzed total housing sales over time using:

Bar Chart
Trend Line
Outlier Detection

Used boxplots to detect potential outliers across numerical features.

Feature Engineering
Encoding
Label Encoding

Applied to:

AREA
STREET
MZZONE
BUILDTYPE
One-Hot Encoding

Applied to:

PARK_FACIL
Ordinal Encoding

UTILITY_AVAIL

AllPub = 3
NoSeWa = 2
NoSewr = 1
ELO = 0

SALE_COND

Normal Sale = 4
AdjLand = 3
Family = 2
Partial = 1
AbNormal = 0
Feature Scaling

StandardScaler applied to:

REG_FEE
COMMIS
Dimensionality Reduction

Principal Component Analysis (PCA) was applied.

The cumulative explained variance plot indicated that:

6 principal components retained most of the variance.
Machine Learning Models

The following regression algorithms were evaluated:

Model
Linear Regression
K-Nearest Neighbors
Decision Tree Regressor
Random Forest Regressor
XGBoost Regressor

Evaluation Metrics:

R² Score
MAE
MSE
Model Selection

Models were compared using R² score.

Best-performing model:

Random Forest Regressor

Hyperparameter tuning was performed using GridSearchCV.

Best Parameters:

criterion='poisson'
max_features=None
min_samples_leaf=1
min_samples_split=3
Power BI Dashboard

The dashboard provides:

Sales Overview
Sales by Area
Sales by Build Type
Sales Trend Analysis
Housing Market Insights

(Add dashboard screenshots here)

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
XGBoost
Power BI
Jupyter Notebook
Project Workflow
Raw Dataset
      ↓
Data Cleaning
      ↓
EDA
      ↓
Feature Engineering
      ↓
Scaling
      ↓
PCA
      ↓
Model Training
      ↓
Hyperparameter Tuning
      ↓
Prediction
      ↓
Power BI Dashboard
CV Project Description

You can put this on your CV:

Developed an end-to-end housing sales analytics solution using Python and Power BI. Performed data cleaning, exploratory analysis, feature engineering, dimensionality reduction (PCA), and predictive modeling using Random Forest and XGBoost. Built an interactive Power BI dashboard to visualize housing market trends and key business insights.
