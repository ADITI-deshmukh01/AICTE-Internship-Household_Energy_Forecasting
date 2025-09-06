# Household Energy Consumption – Week 2 Internship Project

## Project Overview
This project is part of the **AICTE Edunet Foundation Internship** under the theme **Sustainable Energy & Efficiency**.  
The goal of Week 2 is to explore household electricity consumption data, visualize patterns, and analyze daily/weekly trends in energy usage.

## Dataset
We use the **Household Power Consumption Dataset** (sample provided).

| Column                  | Description |
|--------------------------|-------------|
| Date, Time              | Timestamp of measurement |
| Global_active_power     | Total active power consumed (kW) |
| Global_reactive_power   | Reactive power (kW) |
| Voltage                 | Voltage (V) |
| Global_intensity        | Current (A) |
| Sub_metering_1          | Kitchen appliances consumption |
| Sub_metering_2          | Laundry appliances consumption |
| Sub_metering_3          | Water heater & AC consumption |

**Files in the `data/` folder:**
- `household_power_consumption.csv`

## Implementation
- Data loading & preprocessing (Week 1)  
- Daily energy consumption trend analysis (Week 2)  
- Histogram of daily consumption  
- Hourly consumption patterns  
- Insights & observations  

## Observations
- Energy consumption peaks in the evening.  
- Lowest usage is during late night hours.  
- Daily consumption stays within a stable range.  

## Future Work
- Apply ML forecasting models (ARIMA, LSTM).  
- Compare weekdays vs weekends.  
- Integrate weather data for correlation.  

## Files
- `notebooks/Household_Energy_Week2.ipynb`  
- `data/household_power_consumption.csv`
