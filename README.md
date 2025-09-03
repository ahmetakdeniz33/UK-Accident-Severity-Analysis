# UK-Accident-Severity-Analysis
This project explores UK road accident data to understand factors influencing accident severity. Using EDA and a baseline Random Forest model, we analyzed features like Time, Location, Road Type, and Weather. Key predictors include Time, Latitude/Longitude, and Road Number. This provide all analysis, results, and instructions to reproduce the work.
# Capstone Project: UK Accident Severity Analysis

## Project Overview
This project aims to analyze UK road accident data to identify factors that influence accident severity using Exploratory Data Analysis (EDA) and a baseline Machine Learning model (Random Forest).

## Dataset
- Dataset: `UK_Accident.csv`  
- Source: [Available on Kaggle.]  
- Rows: 1,153,399  
- Columns: 32

## Steps Performed
1. Data Cleaning & Preprocessing
   - Converted date columns to datetime
   - Handled missing values
   - Encoded categorical variables
   - Created derived features like `Time_of_Day`

2. Exploratory Data Analysis
   - Correlation heatmaps for numeric features
   - Distribution plots for key features
   - Analysis of accidents by day, month, and location

3. Modeling
   - Baseline model: Random Forest Classifier
   - Train/test split: 70/30
   - Accuracy evaluation and confusion matrix

4. Feature Importance
  Top 15 features influencing Accident Severity:

| Feature                     | Importance |
|------------------------------|------------|
| Time                         | 0.0898     |
| Latitude                     | 0.0815     |
| Location_Northing_OSGR       | 0.0814     |
| Longitude                    | 0.0813     |
| Location_Easting_OSGR        | 0.0810     |
| 1st_Road_Number              | 0.0587     |
| Local_Authority_(District)   | 0.0546     |
| Month                        | 0.0520     |
| Day_of_Week_Name             | 0.0412     |
| Day_of_Week                  | 0.0407     |
| Year                         | 0.0325     |
| Police_Force                 | 0.0257     |
| Number_of_Vehicles           | 0.0240     |
| 2nd_Road_Number              | 0.0191     |

**Insights:**
- **Location** (latitude/longitude) and **time** are the strongest predictors of accident severity.
- Road characteristics and administrative districts also influence severity.
- Non-informative features (like `Unnamed: 0`) were excluded from modeling.
## How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt` (if needed)
3. Open `Accident_Severity_EDA.ipynb` in Jupyter Notebook
4. Run all cells
5. Thank you.

## Author
- Ahmet Akdeniz
- ahmetakdeniz33
