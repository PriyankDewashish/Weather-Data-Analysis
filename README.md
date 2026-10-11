# Weather Data Analysis & Temperature Prediction Using Python

## Project Overview

In this project, I used Python to analyze weather data for 10 Indian cities over six months, from January to June 2025.

I explored temperature, humidity, rainfall, and wind speed to understand how weather conditions differ across cities and change over time. I also created charts to make the results easier to understand.

I also tried a simple way to predict temperature using the previous day's temperature and measured the prediction error using Mean Absolute Error (MAE).

The dataset is synthetic and was created for practice. It does not contain actual weather records.

## Project Objectives

- Clean and analyze weather data using Python.
- Compare temperatures across different cities.
- Analyze rainfall, humidity, and wind speed.
- Study monthly and weekday temperature patterns.
- Explore relationships between weather variables.
- Identify possible temperature outliers.
- Try a simple temperature prediction method and measure its error.

## Tools and Technologies

- **Python** — Used for data analysis.
- **Pandas** — Used to clean, organize, and analyze data.
- **NumPy** — Used for numerical calculations.
- **Matplotlib** — Used to create charts.
- **Seaborn** — Used for statistical charts and correlation heatmaps.
- **Google Colab** — Used to write and run the notebook.
- **Excel (XLSX)** — Used to store the dataset.

## Dataset Description

The dataset contains daily weather records for 10 Indian cities from January 1, 2025, to June 30, 2025.

It includes the following columns:

| Column | Description |
|---|---|
| `Date` | Date of the record |
| `City` | Name of the city |
| `Temperature_C` | Temperature in Celsius |
| `Min_Temperature_C` | Minimum temperature in Celsius |
| `Max_Temperature_C` | Maximum temperature in Celsius |
| `Humidity_Percent` | Humidity percentage |
| `Rainfall_mm` | Rainfall in millimeters |
| `Wind_Speed_kmh` | Wind speed in kilometers per hour |

Some columns contain missing values for data-cleaning practice. The notebook checks for missing values and duplicate records before the analysis.

**Note:** This is simulated data for learning and practice, not actual weather data.

## Data Analysis

I used Pandas to analyze the dataset and Matplotlib and Seaborn to create visualizations.

The analysis includes:

- **Temperature:** Daily trends, average temperatures by city, maximum temperatures, and monthly changes.
- **Rainfall:** Total rainfall by city, monthly rainfall, and rainy-day counts.
- **Humidity:** Average humidity by city and its relationship with temperature.
- **Wind Speed:** Comparison of average wind speed across cities.
- **Correlation:** Relationships between numerical weather variables.
- **Outliers:** Possible temperature outliers identified using the IQR method.
- **Temperature Variation:** Temperature differences across cities and weekdays, along with standard deviation.

## Temperature Prediction

I tested a simple baseline method to predict temperature.

The method uses the previous available day's temperature to predict the current day's temperature for the same city.

For example, if yesterday's temperature was 25°C, the prediction for today would be 25°C.

I calculated the absolute difference between the actual and predicted temperatures and used Mean Absolute Error (MAE) to measure the average prediction error.

The notebook reports an MAE of approximately **2.50°C** on the evaluated data.

This is a simple starting method, not a complete weather forecasting model. The result applies to this synthetic dataset and does not show how accurately the method would predict real weather.

## Key Learnings

Through this project, I practiced:

- Checking and handling missing values.
- Finding duplicate records.
- Cleaning and organizing data using Pandas.
- Grouping data and calculating averages and totals.
- Creating charts using Matplotlib and Seaborn.
- Exploring correlations and possible outliers.
- Using previous values to make a simple prediction.
- Calculating and understanding Mean Absolute Error.

## How to Run the Project

### Option 1: Google Colab

1. Open the notebook in Google Colab.
2. Upload the Excel dataset to Colab.
3. Make sure the dataset file path in the notebook matches the uploaded file.
4. Run the cells from top to bottom.

### Option 2: Run Locally

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. Open the notebook in a Jupyter environment.
5. Make sure the Excel dataset is in the correct location and update the file path if needed.
6. Run the cells from top to bottom.

If Pandas reports that an Excel-reading engine is missing, install `openpyxl` using `pip install openpyxl`.

## Future Improvements

- Repeat the analysis using real historical weather data.
- Compare the baseline with other prediction methods.
- Test prediction performance on a separate period of data.
- Create an interactive dashboard to explore the results.

## Conclusion

This project helped me practice Python data analysis, from cleaning data and creating visualizations to evaluating a simple prediction method.

It improved my understanding of how to explore a dataset, identify patterns, and measure prediction errors. The next step is to apply the same process to real historical weather data.
