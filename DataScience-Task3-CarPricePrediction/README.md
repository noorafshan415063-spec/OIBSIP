# Car Price Prediction Using Machine Learning

## Project Overview
This project focuses on predicting the selling prices of used cars using machine learning techniques. It uses vehicle data from CarDekho and applies data cleaning, exploratory data analysis, feature engineering, and regression models.

## Objectives
- Analyze used car selling prices and related features.
- Clean and prepare the dataset.
- Explore relationships between car features and selling prices.
- Build and evaluate regression models.
- Identify important features influencing model predictions.

## Dataset
**Dataset:** Vehicle Dataset from CarDekho

**Source:** [Kaggle – Vehicle Dataset from CarDekho](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

**Original Dataset Size:** 4,340 rows and 8 columns

**Dataset Size After Cleaning:** 3,577 rows and 8 original columns, with additional engineered features.

### Main Features
- Name
- Year
- Selling Price
- Kilometres Driven
- Fuel
- Seller Type
- Transmission
- Owner

## Technologies and Libraries
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Data Cleaning and Preprocessing
- Checked for missing values.
- Identified and removed 763 duplicate records.
- Created a new feature called `car_age`.
- Extracted car brands from car names.
- Applied One-Hot Encoding to categorical variables.
- Split the dataset into training and testing sets using an 80:20 ratio.

## Exploratory Data Analysis
The project includes visualizations such as:
- Selling price distribution.
- Car age versus selling price.
- Kilometres driven versus selling price.
- Selling price by fuel type.
- Selling price by transmission type.
- Selling price by seller type.
- Selling price by owner type.
- Brand-wise price analysis.
- Correlation heatmap.

## Machine Learning Models

Two regression models were trained:

1. Linear Regression
2. Random Forest Regressor

### Model Evaluation

The models were evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 180,194.99 | 385,606.09 | 0.5384 |
| Random Forest | 157,505.36 | 361,448.67 | 0.5944 |

## Feature Importance
The Random Forest model identified the following as its five most important features:

1. Transmission – Manual
2. Car Age
3. Kilometres Driven
4. Fuel – Diesel
5. Fuel – Petrol

## Conclusion
The Random Forest Regressor performed better than Linear Regression across all three evaluation metrics.

It achieved an R² score of 0.5944, making it the better-performing model for this dataset.

This project provided practical experience in data preprocessing, exploratory data analysis, feature engineering, regression modelling, and model evaluation.

## Project Structure

```text
DataScience-Task3-CarPricePrediction/
│
├── images/
│   ├── 01_selling_price_distribution.png
│   ├── 02_car_age_vs_price.png
│   ├── 03_km_driven_vs_price.png
│   ├── 04_fuel_type_vs_price.png
│   ├── 05_transmission_vs_price.png
│   ├── 06_seller_type_vs_price.png
│   ├── 07_owner_type_vs_price.png
│   ├── 08_brand_vs_price.png
│   ├── 09_correlation_heatmap.png
│   └── 10_feature_importance.png
│
├── NoorAfshan_Task3.ipynb
└── README.md
```

## Author
**Noor Afshan**

Data Science Intern – Oasis Infobyte SIP
