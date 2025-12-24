# 🌦️ Dallas Weather Exploratory Data Analysis (EDA)

This project performs a comprehensive Exploratory Data Analysis (EDA) on weather data from Dallas, Texas, for the year 2024. The goal is to analyze weather patterns, identify correlations between meteorological variables, detect outliers, and visualize key trends such as temperature fluctuations and precipitation.

## 📂 Project Overview

The analysis follows a structured approach to uncover patterns in the data, including:
1.  **Data Inspection**: Understanding the dataset structure, variable types, and summary statistics.
2.  **Data Cleaning**: Handling missing values (particularly in precipitation types) and checking for duplicates.
3.  **Visualization**: Utilizing various plots to explore feature distributions and weather conditions.
4.  **Correlation Analysis**: Examining relationships between numerical variables like temperature, humidity, and wind speed.
5.  **Outlier Detection**: Using Box plots and Interquartile Range (IQR) to identify and address outliers in temperature and precipitation data.

## 📊 Dataset

The dataset used is **Dallas Weather Data (2024)**, containing daily weather observations.

**Key Features:**
* `datetime`: Date of the observation.
* `temp`, `tempmax`, `tempmin`: Average, Maximum, and Minimum temperatures (°F).
* `humidity`: Relative humidity (%).
* `precip`: Precipitation amount (in inches).
* `windspeed` & `windgust`: Wind speed and gust data.
* `conditions`: Categorical description of weather (e.g., Clear, Rain, Partially cloudy).
* `sealevelpressure`: Atmospheric pressure.
* `icon`: Visual representation of the weather condition.

## 🛠️ Technologies & Libraries Used

The project is implemented in Python using a Jupyter Notebook. Key libraries include:

* **Pandas**: For data manipulation and cleaning.
* **NumPy**: For numerical calculations and statistical operations.
* **Matplotlib & Seaborn**: For static visualizations (count plots, histograms, box plots, heatmaps).
* **Plotly Express**: For interactive 3D visualizations.

## 📈 Key Visualizations

The notebook includes several insightful visualizations:
* **Count Plots**: Frequency of different weather conditions and icons.
* **Scatter Plots**: Relationships between Temperature vs. Humidity and Min vs. Max Temperature.
* **Pair Plots**: Pairwise relationships among key numerical variables.
* **Histograms**: Distribution of Temperature and Humidity.
* **Box & Violin Plots**: Analyzing the spread of data and detecting outliers across weather conditions.
* **Heatmap**: Correlation matrix showing the strength of relationships between variables.
* **3D Scatter Plots**: Interactive plots analyzing three variables simultaneously (e.g., Temp vs. Humidity vs. Wind Gust).

## 🚀 How to Run

1.  Clone this repository.
2.  Ensure you have the required libraries installed:
    ```bash
    pip install pandas numpy matplotlib seaborn plotly
    ```
3.  Open the Jupyter Notebook:
    ```bash
    jupyter notebook "EDA on Dallas Weather Data.ipynb"
    ```
4.  Run the cells sequentially to reproduce the analysis.

> **Note**: Ensure the dataset file `Dallas_weather_dataset.csv` is in the same directory as the notebook. The code may reference `/content/Dallas_weather_data.csv` if run originally on Colab; please update the file path in the `pd.read_csv()` function if running locally.
