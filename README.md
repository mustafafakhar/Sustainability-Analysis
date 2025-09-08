# Corporate Energy Consumption Analysis

## Project Overview

This project performs a comprehensive data analysis of corporate energy consumption and emissions. Using historical data, it aims to uncover trends, identify key drivers of energy usage, and provide a forecast of future emissions. This analysis can inform strategic decisions for reducing the corporate environmental footprint and improving sustainability.

## Dataset

The analysis utilizes a publicly available dataset on corporate energy consumption. The key variables include:

- Date: The time of the recorded energy usage.

- Energy Description: The type of energy consumed (e.g., Natural Gas, Electricity, District Energy).

- Emissions(CO2e): The equivalent carbon dioxide emissions in tonnes.

- Other relevant columns from your dataset (e.g., building names, usage metrics).

## Methodology

The project follows a structured data analysis workflow:

- Data Cleaning & Preprocessing: The raw data was cleaned to handle missing values, correct data types, and filter for the most relevant energy sources. A new column was created to represent Emissions(CO2e) for clearer analysis.

- Exploratory Data Analysis (EDA): Key insights were derived by visualizing the data. This included a breakdown of emissions by energy source and an analysis of monthly emission trends.

- Time-Series Forecasting: The Prophet forecasting model was used to predict future emissions. The model was trained on the historical data and configured to account for seasonality and holidays.

- Results & Visualizations: The final output includes a forecast of future emissions and a series of visualizations that tell the story of the data.

## Key Findings

Summarize your most important findings here. For example: Emissions from natural gas are the primary contributor to the total carbon footprint.

Add another key finding, such as: Emissions show a strong seasonal pattern, peaking during winter months due to heating needs.

State the outcome of your forecast, for example: The forecast predicts a gradual increase in emissions over the next 12-24 months unless new energy-saving measures are implemented.

## Visualizations

The following visualizations are key to understanding the project's results:

- Monthly Energy Emissions (Stacked Bar Chart): This chart shows the total monthly emissions, broken down by energy source. It provides a clear view of the seasonal trends and the contribution of each energy type.

- Emissions Forecast: This line plot displays the actual historical emissions alongside the forecasted emissions and their confidence intervals, demonstrating the model's predictive capability.

- Prophet Components: These plots break down the forecast into its core components (trend, yearly seasonality, weekly seasonality), offering deeper insights into the underlying patterns of energy consumption.

## Tools and Libraries

Python: The core programming language for the analysis.

Pandas: Used for data manipulation and cleaning.

Matplotlib & Seaborn: Used for generating static visualizations.

Prophet: A powerful time-series forecasting library developed by Meta.
