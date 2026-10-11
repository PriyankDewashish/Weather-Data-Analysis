# Weather Data Analysis & Temperature Prediction Using Python

## Project Overview

This project explores weather data from multiple Indian cities using Python. It focuses on analyzing temperature, humidity, rainfall, and wind speed to identify patterns, compare weather conditions across cities, and understand relationships between weather variables.

The project also implements a simple baseline temperature prediction method that uses the previous day's temperature to predict the current day's temperature. Its performance is evaluated using Mean Absolute Error (MAE).

The dataset used in this project is **synthetic weather data**, created for learning and analytical practice. It does not represent actual recorded weather conditions.

## Project Objectives

- Analyze temperature patterns across multiple Indian cities.
- Compare average and maximum temperatures across cities.
- Explore rainfall, humidity, and wind speed patterns.
- Identify relationships between weather variables using statistical analysis and visualizations.
- Detect potential temperature outliers using the Interquartile Range (IQR) method.
- Analyze temperature variations by month and day of the week.
- Evaluate a simple temperature prediction baseline using Mean Absolute Error (MAE).

## Tools and Technologies

- **Python** — Core programming language for data analysis.
- **Pandas** — Data cleaning, manipulation, grouping, and aggregation.
- **NumPy** — Numerical operations and statistical calculations.
- **Matplotlib** — Creating charts and visualizations.
- **Seaborn** — Statistical visualizations and correlation heatmaps.
- **Google Colab** — Cloud-based notebook environment.
- **Microsoft Excel format (XLSX)** — Dataset storage and input.

## Dataset Description

The project uses a synthetic weather dataset containing daily weather records for 10 Indian cities from January 1, 2025, to June 30, 2025.

The dataset includes the following columns:

| Column | Description |
|---|---|
| `Date` | Date of the weather record |
| `City` | Name of the city |
| `Temperature_C` | Recorded temperature in Celsius |
| `Min_Temperature_C` | Minimum temperature in Celsius |
| `Max_Temperature_C` | Maximum temperature in Celsius |
| `Humidity_Percent` | Relative humidity percentage |
| `Rainfall_mm` | Rainfall in millimeters |
| `Wind_Speed_kmh` | Wind speed in kilometers per hour |

Missing values were included in selected columns for data-cleaning practice. The notebook checks for missing values and duplicate records before proceeding with the analysis.

**Note:** These are simulated records intended for educational purposes, not actual meteorological observations.

## Analysis and Visualizations

The project explores weather patterns through data analysis and visualizations, including:

- **Temperature Analysis:** Daily temperature trends, average temperatures by city, maximum temperatures, and monthly patterns.
- **Rainfall Analysis:** Total rainfall by city, monthly rainfall patterns, and rainy-day counts.
- **Humidity Analysis:** Average humidity across cities and its relationship with temperature.
- **Wind Speed Analysis:** Comparison of average wind speed across cities.
- **Statistical Analysis:** Descriptive statistics, correlation analysis, temperature outlier detection using IQR, and temperature variability across cities.
- **Time-Based Analysis:** Temperature patterns by weekday and changes over time.

These analyses help explore differences between cities, identify patterns in the synthetic data, and understand relationships between weather variables.

## Temperature Prediction

A simple baseline method is used to evaluate temperature prediction.

### Methodology

- The previous available day's temperature is used as the prediction for the current day.
- Predictions are calculated separately for each city.
- The absolute difference between actual and predicted temperatures is calculated.
- Mean Absolute Error (MAE) is used to evaluate the prediction results.

### Evaluation Metric

**Mean Absolute Error (MAE)** measures the average absolute difference between actual and predicted temperatures. A lower MAE indicates smaller prediction errors.

The notebook's saved result reports an MAE of approximately **2.50°C**. This is a baseline result on the synthetic dataset and should not be interpreted as evidence of real-world weather forecasting accuracy.

## How to Run the Project

1. Clone or download this repository.

2. Ensure Python is installed, or open the notebook in Google Colab.

3. Install the required libraries if they are not already available:

   ```bash
   pip install pandas numpy matplotlib seaborn 
   ```

4. Keep the Excel dataset in the same directory as the notebook, or update the dataset file path in the code.

5. Open the notebook and run the cells from top to bottom.

The notebook performs data inspection, cleaning, exploratory analysis, visualization, and baseline temperature prediction.

## Key Takeaways

- Explored temperature, rainfall, humidity, and wind speed across multiple cities.
- Practiced handling missing values and checking for duplicate records.
- Used statistical summaries and visualizations to investigate weather patterns.
- Applied the IQR method to identify potential temperature outliers.
- Evaluated a simple temperature prediction baseline using MAE.
- Gained practical experience with Python-based exploratory data analysis.

The findings describe patterns in the synthetic dataset and should not be treated as conclusions about actual weather conditions.

## Future Improvements

- Use real historical weather data for more meaningful analysis.
- Compare multiple baseline and machine-learning prediction methods.
- Evaluate prediction performance on a separate test period.
- Add interactive dashboards for exploring weather patterns.
- Investigate seasonal patterns and relationships between additional weather variables.