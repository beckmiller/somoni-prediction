# Prediction Tajikistan local currency
This is the time series analysis of Tajikistan local currency somoni (TJS). Here I used several famous predictions models such as Holt-Winters, ARIMA, SARIMAX and etc. Then I compare each model.

## :open_file_folder: Dataset

The dataset used is the [National Bank of Tajikistan](https://nbt.tj/ru/kurs/kurs.php) rate of USD/TJS dataset. This dataset contains rate of currencies data from 2001 to 2022 sampled everyday. I decided to resample the dataset with monthly frequency for both easier data handling and proximity to a real use case scenario (because NBT raises rate monthly, quaterly, semi-annually). In this case the series is not stationary with some small seasonalities(seasonal) which change every year(quaterly).

## :triangular_ruler: Models tested

* Holt-Winters ExponentialSmoothing ([HWE](https://www.statsmodels.org/dev/generated/statsmodels.tsa.holtwinters.ExponentialSmoothing.html))
* Seasonal autoregressive integrated moving average ([SARIMA](https://www.statsmodels.org/dev/generated/statsmodels.tsa.statespace.sarimax.SARIMAX.html))

## :mag: Forecasting results
There are several popular models left, like LSTM, XGBoost, Prophet, Lasso and etc. that I should implement.

### Evaluation Metrics
* Root Mean Squared Error (RMSE)
* Mean Absolute Percentage Error (MAPE)
<table class="table table-bordered table-hover table-condensed">
<thead><tr><th title="Field #1">Model</th>
<th title="Field #3">rmse</th>
<th title="Field #3">mape</th>
</tr></thead>
<tbody><tr>
<td>SARIMA</td>
<td align="right">0.48</td>
<td align="right">0.04</td> 
</tr>
<tr>
<td>Holt-Winters</td>
<td align="right">0.41</td>
<td align="right">0.03</td> 
</tr>
