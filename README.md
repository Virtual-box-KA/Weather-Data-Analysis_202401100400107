# Weather-Data-Analysis_202401100400107
# Weather Data Analysis - Visualizing Temperature Trends, Rainfall, and Seasonal Patterns

## Overview

This project analyzes a weather dataset of Seattle city, providing visualizations of temperature trends, precipitation, wind speed, and weather conditions. The dataset is analyzed using Python libraries like `Pandas`, `Matplotlib`, and `Seaborn` to visualize key weather patterns over time.

## Project Details

- Technologies Used:
  - Python
  - Pandas
  - Matplotlib
  - Seaborn
  - Time (for implementing delays in visualization)

- Dataset:
  - Source: [Kaggle - Seattle Weather Data](https://www.kaggle.com/datasets/ananthr1/weather-prediction/data)
  - Content: The dataset contains daily weather data of Seattle with columns for:
    - Date
    - Precipitation
    - Maximum Temperature
    - Minimum Temperature
    - Wind Speed
    - Weather Condition

---

## **Installation**

To run the project, follow these steps:

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/weather-data-analysis.git
```

2. **Navigate to the project folder:**

```bash
cd weather-data-analysis
```

3. **Install the required dependencies:**

If you don't have the required libraries, you can install them using `pip`:

```bash
pip install pandas matplotlib seaborn
```

---

## Usage

1. Download the Dataset:

   - Download the dataset from [Kaggle](https://www.kaggle.com/datasets/ananthr1/weather-prediction/data) and place the `Seattle-weather.csv` file in the project directory.

2. Run the Script:

   You can run the Python script by executing the following command:

```bash
python weather_analysis.py
```

3. Visualizations:

   The script will load the dataset and generate the following plots:
   
   - Temperature Trends: Line plot showing the maximum and minimum temperatures over time.
   - Precipitation Distribution: Histogram displaying the distribution of precipitation.
   - Wind Speed Distribution: Histogram showing the distribution of wind speed.
   - Weather Condition Frequency: Count plot illustrating the frequency of different weather conditions.

4. Output:
   The generated plots will appear sequentially, with a slight delay before each plot is shown (to simulate thinking time).

---

## Code Explanation

### 1. Data Preprocessing

The dataset is loaded using `pandas.read_csv()`, and the "date" column is converted to a `datetime` format using `pd.to_datetime()`. Any missing data is handled appropriately, and a summary of the data is displayed.

### **2. Visualization**

The following plots are generated:

- Temperature Trends: A line plot that shows the maximum and minimum temperature for each day. It helps analyze seasonal variations in temperature.
  
- Precipitation Distribution: A histogram that illustrates the distribution of daily precipitation, identifying the most common and extreme rainfall events.
  
- Wind Speed Distribution: A histogram that shows the distribution of wind speeds, highlighting the most common wind speeds and any extreme occurrences.

- Weather Condition Frequency: A count plot that displays the frequency of each weather condition in the dataset.

### 3. Delays in Plotting

A custom function `show_plot_with_delay()` is used to simulate thinking before displaying each plot. This function includes a 2-second delay (`time.sleep(2)`) before displaying each plot.

---

## Key Observations

- Temperature Trends: The line plot reveals fluctuations in the maximum and minimum temperatures, showing the seasonal variations in Seattle's weather.
  
- Precipitation: Most days recorded little to no precipitation, with a few instances of high rainfall.

- Wind Speed: The distribution of wind speeds suggests that most wind speeds are moderate, with rare occurrences of high-speed winds.

- Weather Conditions: The count plot highlights that certain weather conditions (like "Clear" and "Rain") are more common than others.

---

## Challenges & Future Improvements

- Challenges:
  - Data preprocessing (handling missing values and ensuring correct data types).
  - Ensuring accurate and meaningful visualizations.

- Improvements:
  - Enhance the visual appeal of the plots (e.g., using more attractive themes, colors, and interactivity).
  - Build a web-based dashboard for better user interaction.
  - Integrate machine learning models to predict future weather trends based on historical data.

---

## Conclusion

This weather data analysis provides valuable insights into the weather patterns of Seattle. It can be applied in various fields such as agriculture, construction, and climate study to aid decision-making processes.

---

## References

- Data: [Kaggle - Seattle Weather Data](https://www.kaggle.com/datasets/ananthr1/weather-prediction/data)
- Code Resources:
  - [Pandas Documentation](https://pandas.pydata.org/)
  - [Matplotlib Documentation](https://matplotlib.org/)
  - [Seaborn Documentation](https://seaborn.pydata.org/)
