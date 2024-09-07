# Yulu Bike Rental Demand Analysis

## Project Overview

Yulu, a leading micro-mobility service provider in India, has been experiencing a decline in revenues. To address this issue, this project aims to identify the key factors influencing the demand for shared electric cycles in the Indian market. The analysis leverages a dataset containing bike rental records and various environmental and temporal variables. By applying statistical methods, the project seeks to uncover insights that can help Yulu optimize its services.

## Objectives

- Identify significant variables that predict bike rental demand.
- Evaluate the descriptive power of these variables.
- Understand how factors such as weather, season, holidays, and working days affect bike rental demand.
- Provide actionable insights to enhance Yulu's micro-mobility services.

## Dataset

The dataset used in this analysis includes the following variables:

- `datetime`: Date and time of the record.
- `season`: Season (1: Spring, 2: Summer, 3: Fall, 4: Winter).
- `holiday`: Whether the day is a holiday.
- `workingday`: Whether the day is a working day.
- `weather`: Weather condition (1: Clear, 2: Mist, 3: Light rain/snow, 4: Heavy rain/snow).
- `temp`: Temperature in Celsius.
- `atemp`: "Feels like" temperature in Celsius.
- `humidity`: Humidity percentage.
- `windspeed`: Wind speed.
- `casual`: Number of casual users.
- `registered`: Number of registered users.
- `count`: Total number of bike rentals.

## Analysis

### 1. Exploratory Data Analysis (EDA)
- **Graphical Analysis**: Visualized the distribution of variables and relationships between them using histograms, bar plots, and pie charts.
- **Outlier Detection**: Identified and treated outliers in temperature, wind speed, and humidity using box plots and percentile-based clipping.

### 2. Statistical Testing
- **Two-sample T-Test**: Tested if there is a significant difference in bike rentals on weekdays vs. weekends.
- **ANOVA and Kruskal-Wallis H-Test**: Analyzed whether bike rental demand differs significantly across weather conditions and seasons.
- **Chi-Square Test**: Examined the dependency between weather and season.

### 3. Findings
- **Seasonal Demand**: Higher demand in spring and summer, with a decline in fall and winter.
- **Weather Impact**: Clear or cloudy weather saw higher rentals, while extreme weather conditions led to fewer rentals.
- **Working vs. Non-Working Days**: No significant difference in rental demand.
- **Temperature and Humidity**: Most rentals occurred when temperatures were below 28°C and humidity was above 40%.

### 4. Recommendations
- **Seasonal Pricing**: Implement dynamic pricing based on seasonal demand.
- **Weather-based Promotions**: Offer discounts or incentives during adverse weather to boost rentals.
- **Operational Efficiency**: Focus on peak rental hours and optimize bike availability accordingly.

## Conclusion

This analysis provides Yulu with critical insights into the factors affecting bike rental demand. By leveraging these findings, Yulu can optimize its operations and potentially reverse the decline in revenues.

## Dependencies

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
