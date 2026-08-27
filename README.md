# used-car-price-eda
EDA + Feature Engineering on Used Car Price dataset - LearnDepth internship

# Used Car Price Prediction — EDA & Feature Engineering

## Overview
This project performs exploratory data analysis (EDA) and feature engineering on a 
used-car dataset to understand which factors are most strongly associated with 
resale price. This was completed as part of my internship project at **LearnDepth**.

## Dataset
- **File:** `09_used_car_price.csv`
- **Rows:** 1000 (before cleaning)
- **Columns:**
  - `car_age_years` — age of the car in years
  - `km_driven` — total kilometers driven
  - `engine_cc` — engine size in cc
  - `owners` — number of previous owners
  - `price_lakh` — resale price (target variable)

## Tools & Libraries
- Python
- pandas
- numpy
- matplotlib
- seaborn
- Google Colab (development environment)

## Project Workflow
1. Loaded and inspected the dataset (shape, dtypes, summary statistics)
2. Checked for missing values and duplicate rows
3. Identified invalid values using boolean filtering (negative age, negative 
   kilometers, unrealistic owner counts, negative/zero prices)
4. Visualized distributions and outliers using histograms and boxplots
5. Compared key features against price using scatterplots
6. Built a correlation heatmap to quantify feature relationships
7. Cleaned the dataset (removed duplicates and invalid rows, filled missing 
   values with median)
8. Engineered two new features: `km_per_year` and `is_high_mileage`
9. Re-checked the cleaned dataset
10. Separated features (X) and target (y) for future modeling

## Key Findings
- **car_age_years** had the strongest correlation with price (**-0.67**) — 
  older cars are worth less.
- **km_driven** had the second strongest correlation (**-0.54**) — higher 
  mileage lowers resale price.
- **engine_cc** showed a weak correlation (**0.13**).
- **owners** showed almost no correlation (**-0.01**).
- After cleaning, the dataset was reduced from 1000 to 938 valid rows.

## Files in this Repository
- `used_car_price_eda.ipynb` — full notebook with code, outputs, and charts
- `used_car_price_eda.py` — plain Python script version
- `Used_Car_Price_EDA_Report.docx` — full project report/documentation

## Author
**Manahil** — BSAI Student, Air University
