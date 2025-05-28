# ⚡ Integrated Energy & Weather Intelligence Dashboard

This Power BI project analyzes how weather conditions influence energy consumption and renewable power production across Spain. It leverages two interconnected datasets—energy and weather—to deliver an interactive dashboard for decision-makers, energy analysts, and researchers.

## 📌 Project Overview

An end-to-end data pipeline was developed:

- **Data Source**: Datasets from Kaggle (`energy_dataset.csv`, `weather_features.csv`)
- **Storage**: Imported and structured in MySQL
- **Visualization**: Connected to Power BI to build a 3-page dashboard with slicers, bookmarks, and visuals

## 🎯 Aim

To create an interactive Power BI dashboard that:
- Monitors energy consumption & production
- Compares forecast vs. actual energy loads
- Examines the impact of weather conditions
- Supports sustainable, data-driven energy decisions

## ❓ Problem Statement

Accurately managing energy resources is challenging due to:
- Unpredictable weather patterns
- Limited integration of weather and energy insights in traditional tools
This project addresses that by combining both datasets to visualize trends, improve forecasting, and drive efficient energy decisions.

## 🔍 Research: Energy Consumption in Spain

Spain exhibits seasonal energy demand, with peaks in winter and summer. The country relies heavily on renewables (wind, solar, hydro), whose output is weather-dependent. Accurate forecasting and real-time monitoring are essential to maintain grid balance and sustainability.

## 🗂 Data Source

- **Energy Dataset** (Kaggle):  
  Hourly energy generation, consumption, forecast data  
- **Weather Dataset** (Kaggle):  
  Hourly weather metrics across cities (temperature, humidity, wind speed, etc.)

## 🛠️ Data Cleaning

- Removed null/duplicate entries
- Standardized datetime fields
- Merged datasets using `datetime` and `city`
- Created calculated fields like:
  - Load Difference = Actual - Forecast
  - Time Hierarchies: Hour, Day, Month
- Replaced missing values and filtered unnecessary columns

## 🎯 Target Audience

- Energy analysts
- Utility managers
- Policy makers
- Data science students
- Business stakeholders in energy sector

## ✨ Key Features

- Interactive 3-page Power BI dashboard
- Actual vs. forecast load comparison
- Weather trend impact on renewable generation
- KPIs, slicers, buttons, bookmarks
- Visuals: line charts, stacked areas, donut charts, cards, gauges

## 📊 Reports

### 🔹 Page 1 – Energy Overview
- Comparison of forecast vs. actual load
- Stacked area chart: solar, wind, hydro contributions
- KPIs for energy trends and demand peaks

### 🔹 Page 2 – Weather Impact Analysis
- City-wise weather trends: temperature, humidity, wind
- Scatter plots: wind speed vs. wind energy
- Correlations between weather and consumption

### 🔹 Page 3 – Integrated Dashboard
- Combined visuals: load, forecast, weather metrics
- Filters: date, city, weather type, energy source
- Cards, donut charts, line trends for detailed insights

## 🚧 Project Scope

- Focused on Spain
- Examines energy–weather relationship
- Enables real-time filtering and decision making

### 🔒 Limitations

- Dataset limited by time & cities
- Renewable data not device-specific
- No real-time streaming or weather extremes

## ✅ Expected Outcome

- Reveal forecast accuracy and gaps
- Correlate weather to demand and renewables
- Empower analysts with interactive decision-making tools

## 🚀 Future Enhancements

- Live data with APIs
- Machine learning forecasting
- Country-wise comparison
- Drill-through pages, dark mode, export options

## 🔄 Pipeline Overview

```text
Kaggle → MySQL → Power BI
