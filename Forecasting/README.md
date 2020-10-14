# Forecasting
Perform forecasting with [FBProphet](https://facebook.github.io/prophet/), LSTM with [Keras](https://keras.io/), and [Holt's Method](https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html#Holt's-Method) on single time series. 

Forecasting plays an important role across various fields and industries, including but not limited to Manufacturing, DevOps, and IoT. Forecasting enables better [production planning](https://en.wikipedia.org/wiki/Production_planning#:~:text=Production%20planning%20is%20the%20planning,order%20to%20serve%20different%20customers.), [capacity planning](https://en.wikipedia.org/wiki/Capacity_planning#:~:text=Capacity%20planning%20is%20the%20process,completing%20in%20a%20given%20period.), as well as [predictive maintenance](https://en.wikipedia.org/wiki/Predictive_maintenance).   

## About FBProphet

FBProphet or [Prophet](https://facebook.github.io/prophet/) is a forecasting time series library. The Prophet frames the forecasting problem as a curve-fitting exercise. It is an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. Prophet is best suited for time series data with strong seasonality. Ideally you can fit an entire cycle of historical data or several seasons of historical data. 

## About LSTM 

[LSTM](https://en.wikipedia.org/wiki/Long_short-term_memory) or Long short-term memory is an artificial recurrent neural network (RNN). [Understanding LSTM Networks](http://colah.github.io/posts/2015-08-Understanding-LSTMs/) is a fantastic resource to those wanting to learn more about how LSTMs work. 

## About Holt's Method 
[statsmodels](https://www.statsmodels.org/stable/about.html#about-statsmodels) is a Python module that provides functions for many statistical models (including forecasting and anomaly detection) and statistical data exploratin. The [statsmodels Holt's method](https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html#Holt's-Method) is used to generate forecasts. Holt's method is also known as double exponential smoothing. Double exponential smoothing is an exponentially weighted average of the trend and values of the data together. To learn about how to implement this forecasting method with the Telegraf Execd processor plugin, 