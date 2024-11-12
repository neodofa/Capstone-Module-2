# NYC Taxi Demand Analysis - Capstone Project

## Project Overview
This project provides an in-depth analysis of taxi demand in New York City, using data-driven insights to identify peak demand times, high-demand locations, and the key factors influencing trip characteristics such as distance, duration, fare, and tips. The project’s objective is to support data-informed decisions in fleet management, pricing strategies, and service optimization.

## Dataset
The dataset used in this project includes detailed records of NYC taxi trips, with fields such as:
- `pickup_datetime` and `dropoff_datetime`
- `trip_distance`
- `fare_amount`, `tip_amount`, and `total_amount`
- `PULocationID` and `DOLocationID` for pickup and dropoff locations
- `passenger_count`

## Project Structure
The analysis is conducted in a Jupyter Notebook (`capstoneproject.ipynb`) and follows these main steps:

1. **Data Cleaning**: 
   - Handled missing values, removed duplicates, and addressed outliers to ensure data quality.
   - Calculated `trip_duration` in minutes as the difference between `dropoff_datetime` and `pickup_datetime`.

2. **Exploratory Data Analysis (EDA)**:
   - **Temporal Analysis**: Analyzed trip frequency by hour and day of the week to identify peak demand times.
   - **Spatial Analysis**: Examined pickup locations to locate high-demand areas in NYC.
   - **Trip Characteristics**: Explored distributions of trip distance, fare amount, and trip duration.

3. **Correlation Analysis**:
   - Calculated correlations between `trip_distance`, `trip_duration`, `fare_amount`, and `tip_amount`.
   - Visualized correlations with a heatmap to understand relationships among key variables.

4. **Outlier Detection and Handling**:
   - Identified and handled outliers in `trip_distance`, `fare_amount`, `tip_amount`, and `passenger_count` using Z-scores.

5. **Visualization**:
   - Created visualizations to illustrate demand patterns, trip characteristics, and correlation insights.

## Key Insights
- **Peak Demand Times**: Taxi demand peaks between 3 PM and 6 PM on weekdays, with Tuesdays showing the highest volume.
- **High-Demand Locations**: Key pickup locations align with business districts and transportation hubs, indicating strategic areas for fleet allocation.
- **Trip and Fare Patterns**: Strong correlation between `trip_distance` and `fare_amount`, highlighting a distance-based pricing structure. Tips tend to increase with higher fares and longer distances, though the correlation is moderate.

## Recommendations
- **Fleet Management**: Prioritize fleet availability in high-demand areas during peak hours on weekdays, especially on Tuesdays.
- **Pricing Strategy**: Consider incentives for longer trips to encourage tipping and optimize fare revenue.

## Getting Started
To run the analysis:
1. Clone this repository and navigate to the project folder.
2. Install the required libraries by running:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
