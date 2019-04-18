# beachwaterqualitytimeseries
Time Series Forecasting of E.Coli counts using Python and Data Science Tools (Pandas, matplotlib, statsmodels etc)

**Tasks completed thus far:**
* Extracted and cleaned raw XML weather data and e. Coli count data (~1000 data points)
* Analyzed e. Coli counts in the past 10 years over 11 beaches around Toronto (~920 datapoints)
* Performed day-by-day differencing to check for stationarity in the data before modeling
* Predicted single data point forecast and compared against expanded forecast using the statsmodels ARIMA model with parameters (AR=6, D=1, MA=1)
* Programmed the ARIMA model to forecast using 30% of the dataset based on a training dataset of 70%
* Calculated RMSE values of the ARIMA model for both forecasts
* Results: RMSE IQR doubled after including more datapoints; RMSE median tripled as well.

**TASKS TODO:**
* Investigate why the IQR and median values are increasing with increasing number of datapoints in the forecast
* Conduct log/sqrt transformations for the E.coli counts of each beach
* Check whether transformations change the data to fit them better with a normal distribution
* Change the parameters of the ARIMA model, leveraging MA model more (this is currently set only to q=1)
