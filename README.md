# Rainfall Prediction and Analysis in India (IMD Data)

This project performs a comprehensive analysis and prediction of rainfall patterns across various subdivisions in India using historical data from the India Meteorological Department (IMD). It utilizes Python's data science stack to clean data, perform exploratory analysis, and build regression models for future predictions.

## Project Overview

Rainfall is a critical factor for India's economy and agriculture. This project aims to:
- **Analyze** historical rainfall trends (1901–2017).
- **Visualize** seasonal and monthly variations across different regions.
- **Predict** future rainfall using machine learning algorithms.

## Dataset

The project uses the `Sub_Division_IMD_2017.csv` dataset, which contains:
- **SUBDIVISION**: The specific region in India.
- **YEAR**: Data spanning from 1901 to 2017.
- **Monthly Rainfall**: (JAN to DEC).
- **Annual Rainfall**.
- **Seasonal Subsets**: JF (Jan-Feb), MAM (Mar-May), JJAS (Monsoon), OND (Oct-Dec).

## Features

- **Data Cleaning**: Handling missing values using mean imputation and stripping whitespace from categorical data.
- **Feature Engineering**: Creation of new columns for major seasons:
    - `MONSOON` (Jun-Sep).
    - `WINTER` (Dec-Feb).
    - `SUMMER` (Mar-May).
    - `DECADE` (grouping by 10-year periods).
- **Exploratory Data Analysis (EDA)**: Statistical summaries and visualizations using Matplotlib and Seaborn.
- **Machine Learning**: 
    - **Linear Regression**: For simple trend prediction.
    - **Random Forest Regressor**: For more robust, non-linear predictions.
    - **K-Means Clustering**: To group regions based on rainfall similarities.

## Tech Stack

- **Language**: Python
- **Libraries**: 
  - `Pandas` & `NumPy` for data manipulation.
  - `Matplotlib` & `Seaborn` for data visualization.
  - `Scikit-learn` for preprocessing and machine learning models.

