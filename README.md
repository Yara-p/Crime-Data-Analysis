# Crime Data Analysis

## Project Overview
This project focuses on analyzing crime data from Los Angeles between January 1, 2020, and October 16, 2023. The analysis explores crime trends, seasonal patterns, crime type distribution, correlations with economic factors, and demographic influences on crime. Time series models were also implemented to predict future crime rates based on historical data.

## Data Source
The crime data was sourced from the [U.S. Government Open Data Portal](https://catalog.data.gov/dataset/crime-data-from-2020-to-present), which provides detailed records of crime occurrences, victim demographics, crime types, and geographic information.

## Key Components
1. **Data Cleaning & Preprocessing**:
   - Handled missing values by filling relevant fields with 'unknown' and removed extraneous columns.
   - Converted crime occurrence dates to datetime format for time series analysis.
   - Outlier detection on victim age using box plot analysis.

2. **Exploratory Data Analysis (EDA)**:
   - **Crime Trends**: Analyzed the escalation of crime rates, peaking in 2022, followed by a decline in 2023.
   - **Seasonal Patterns**: Crime incidents tend to peak during the summer months, particularly in July.
   - **Top Crime Types**: 'Vehicle Stolen' and 'Battery-Simple Assault' were identified as the most frequent crime types.
   - **Geographic Trends**: Higher crime rates in the Central area, with lower rates in the Foothill region.
   
3. **Correlation with Economic Factors**:
   - **Unemployment Rate**: A moderate negative correlation (-0.67) was found, suggesting that higher unemployment may coincide with lower crime rates.
   - **CPI-U**: A strong positive correlation (0.79) was observed between consumer prices and crime rates.
   - **Inflation Rate**: Exhibited a weak positive correlation with crime numbers.
   - **Mortgage Delinquency Rate**: Showed no significant correlation with crime rates.

4. **Demographic Factors**:
   - **Gender**: Males were slightly more prone to crime, with notable exceptions for crimes like identity theft, where females were more affected.
   - **Age**: Victims in the 20-40 age range were most vulnerable, with specific crime types such as identity theft and robbery predominant in these groups.

5. **Time Series Analysis & Prediction**:
   - Implemented **SARIMA**, **ARIMA**, and **LSTM** models to predict future crime rates, with the **SARIMA** model providing the best fit based on AIC values.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/crime-data-analysis.git
