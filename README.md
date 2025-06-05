# Aircraft Market Risk Profiling & Volatility Analysis

This project analyzes volatility and operational risk in the U.S. domestic airline market using flight performance data. By applying time-series analysis, we profile flight frequency trends and arrival delay variability to identify instability patterns and high-risk carriers.

## Project Objectives

- Identify volatility patterns across airline carriers using standard deviation of arrival delays.
- Model order frequency and transactional variance through time-series analysis.
- Visualize trends and risk exposures using clear, data-driven dashboards.

## Data Source

The dataset comes from [Kaggle: flights.csv](https://www.kaggle.com/datasets), which contains U.S. domestic flight information for the year 2013, including:
- Carrier code, delay time, departure/arrival times, and flight counts.
- Timestamps (`time_hour`) for time-series resampling.

## Key Visualizations

### 1. Arrival Delay Volatility by Airline
Bar chart showing the standard deviation of arrival delays for each airline carrier.
> Airlines with higher standard deviations exhibit greater inconsistency in performance, indicating higher operational risk. Hawaiian Airlines (HA) shows the highest volatility, while US Airways (US) is the most stable.

### 2. Flight Frequency Over Time
Time-series plot of daily flight counts and 7-day moving average.
> Weekly seasonality and long-term trends are clearly visible. Flight frequency increases from March to July (peak season), then drops post-September. Sharp dips in June, July, and December suggest potential disruptions or seasonal adjustments.

### 3. Arrival Delay Volatility Over Time
Time-series chart showing daily standard deviation and 7-day rolling coefficient of variation (CV), with a threshold filter applied to remove CV outliers.
> This chart helps reveal periods of unusually high delay variability, highlighting instability windows in the market.

## Tools Used

- **Python**: Data analysis & visualization
- **Pandas**: Data manipulation and resampling
- **Matplotlib**: Plotting
- **Time-Series Techniques**: Rolling window analysis, volatility modeling, threshold-based CV filtering

## Insights

- Volatility varies significantly across carriers, suggesting varying operational risk profiles.
- Weekly flight frequency patterns confirm strong operational seasonality.
- Delay volatility spikes can highlight market stress periods or external disruptions.

## Next Steps (Optional)

- Extend analysis by adding carrier-specific breakdowns
- Introduce external variables (e.g., weather, holidays)
- Build a real-time dashboard using Plotly or Power BI

## Repository Structure

