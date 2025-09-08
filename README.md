# AICTE Internship – Household Energy Forecasting

## Project Overview
This project is part of the AICTE Edunet Foundation Internship under the theme **Sustainable Energy & Efficiency**.

The goal of Week 1 & Week 2 is to explore household energy consumption data, visualize trends, and analyze daily usage patterns.

## Dataset
The dataset contains household power consumption measurements:

| Column | Description |
|--------|-------------|
| Date   | Measurement date |
| Time   | Measurement time |
| Global_active_power | Household global active power (kilowatts) |
| Global_reactive_power | Household global reactive power (kilowatts) |
| Voltage | Voltage (volts) |
| Global_intensity | Intensity (ampere) |
| Sub_metering_1 | Energy sub metering 1 |
| Sub_metering_2 | Energy sub metering 2 |
| Sub_metering_3 | Energy sub metering 3 |

## Implementation
- Loaded and explored the dataset using Pandas.
- Checked dataset info, shape, and missing values.
- Converted Date + Time into a datetime column.
- Plotted daily energy consumption trends.
- Plotted distribution of daily usage.
- Added observations summarizing key patterns.

## Observations
- Energy usage varies daily depending on household activity.
- Peak usage occurs during evening hours.
- Weekend vs weekday consumption may show different behavior.

## Future Work
- Apply ML forecasting models (ARIMA, LSTM).
- Compare weekdays vs weekends consumption patterns.
- Integrate weather data for better correlation with energy usage.
