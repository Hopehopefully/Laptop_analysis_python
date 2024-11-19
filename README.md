# Laptop_analysis_python

## 1. Overview
This project focuses on analyzing a dataset of laptops to explore relationships between features such as RAM, weight, and price. The main objectives are to clean the data, calculate derived metrics, and perform predictive modeling to estimate laptop prices based on features. Additionally, visualizations like 3D scatter plots and pivot tables are used to highlight key trends and comparisons within the data.

## 2. Data Cleaning
This section outlines the data preprocessing steps taken to prepare the dataset for analysis:

Handling Missing and Null Values: Missing values in the "Operating System Version" column were filled with "Unknown." Blank or whitespace-only rows were identified to ensure dataset completeness.
Feature Formatting: String features like "RAM," "Screen Size," and "Weight" were converted to numerical formats by removing units (e.g., "GB," "kg") and casting them to appropriate data types.
Summary Statistics and Missing Value Check: Descriptive statistics were computed for numerical features to understand data distributions, and missing values were identified and addressed where necessary.
Filling Missing Prices: Missing values in the "Price" column were filled with the column's mean value to maintain consistency.
## 3. Feature Engineering
This section describes the creation of new features to enhance analysis:

Price per GB of RAM: A derived metric was created to show how price scales with the amount of RAM in each laptop.
Screen Area: A new feature was calculated to estimate the physical screen area of laptops, assuming a 16:9 aspect ratio.
## 4. Predictive Modeling
A simple linear regression model was implemented to predict laptop prices based on RAM and weight. Key details include:

Model Coefficients: The slopes (coefficients) for RAM and weight were calculated using linear regression formulas, and the intercept was determined.
Predicted Prices: The model outputs a new column, "Predicted Price," to compare against actual prices in the dataset.
## 5. Data Visualization
Various visualizations were created to better understand the data and validate predictions:

3D Scatter Plots: A 3D plot compares actual laptop prices with predicted prices based on RAM and weight.
2D Scatter Plots: Scatter plots show the relationship between RAM and both actual and predicted prices, highlighting the model's performance.
Pivot Table: A pivot table summarizes average laptop prices by manufacturer and category for quick comparisons.
## 6. Analysis Highlights
Key insights and analyses derived from the dataset include:

Correlation Analysis: A correlation matrix was generated to explore relationships among numerical features (e.g., RAM, weight, price).
Average Price by Manufacturer and Category: Grouped averages highlight which manufacturers and categories have the highest and lowest prices.
Comparison of Actual vs Predicted Prices: The model's predictions are compared against the actual values to assess accuracy and identify trends.
## 7. Quality Assurance
Checks were performed to ensure data quality and model accuracy:

NaN and Infinite Value Checks: Columns were examined for missing or infinite values to avoid errors in computation.
Total Missing Values: The project quantified the total number of missing values to gauge dataset quality.
## 8. Conclusion
The project provides a cleaned and enriched dataset ready for further exploration or more sophisticated predictive modeling. Visualizations and metrics offer insights into price trends and relationships among features. The repository serves as a foundation for anyone interested in working with consumer electronics data or applying predictive modeling techniques to structured datasets.
