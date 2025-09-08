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
The following are the key findings of the analysis:

- Analysis of the historical data shows a seasonality trend, which means that every year during a certain period of time, the emissions increase and decrease. This could either be due to increased demand of heating during the winter season. The winters in Canada are extremely cold or energy requirement in the country during the season.
- The Prophet forecast model shows a clear and strong annual seasonality. The peaks are observed at the same time each year, likely presenting a period of high emissons and the drops in the peak showing reduction of energy consumption.
- The trend in the data appears to be relatively flat. There is no significant long-term increase or decrease in energy consumption. This can also be observed in the future forecasted model. This, therefore, suggests that there is no significant change in trajectory in the established seasonal patterns.
- The light blue shaded area represents the uncertainty interval of the forecast. This interval widens over time, which is typical for time-series forecasts. The increasing width indicates that the model is less certain about its predictions further into the future. The black dots show the actual historical data points, and most of them fall within the uncertainty band, which suggests the model is a good fit for the historical data
- There are a few outliers visible as black dots that fall outside the main pattern. For example, some data points are lower than the rest, while others are higher. The model's prediction line smooths over these anomalies, focusing on the underlying trend and seasonality. This is a common feature of Prophet, as it is designed to be robust to outliers.


## Visualizations

The following visualizations are key to understanding the project's results:

- Monthly Energy Emissions (Stacked Bar Chart): This chart shows the total monthly emissions, broken down by energy source. It provides a clear view of the seasonal trends and the contribution of each energy type.

- Emissions Forecast: This line plot displays the actual historical emissions alongside the forecasted emissions and their confidence intervals, demonstrating the model's predictive capability.

- Prophet Components: These plots break down the forecast into its core components (trend, yearly seasonality, weekly seasonality), offering deeper insights into the underlying patterns of energy consumption.

## Tools and Libraries

- Python

- Pandas

- Matplotlib & Seaborn: Used for generating static visualizations.

- Prophet: A powerful time-series forecasting library developed by Meta.

