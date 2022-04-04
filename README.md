# Prediction Tajikistan local currency
## :open_file_folder: Dataset

The dataset used is the [National Bank of Tajikistan](https://nbt.tj/ru/kurs/kurs.php) rate of USD/TJS dataset. This dataset contains rate of currencies data from 2001 to 2022 sampled everyday. I decided to resample the dataset with monthly frequency for both easier data handling and proximity to a real use case scenario (because NBT raises rate monthly, quaterly, semi-annually). In this case the series is not stationary with some small seasonalities(cyclic) which change every year(quaterly).

This is the time series analysis of Tajikistan local currency somoni (TJS). Here I used several famous predictions models such as Holt-Winters, ARIMA, SARIMAX and etc. Also tried to compare each other.
## :triangular_ruler: Models tested

* Holt-Winters ExponentialSmoothing ([HWE](https://www.statsmodels.org/dev/generated/statsmodels.tsa.holtwinters.ExponentialSmoothing.html))
* Seasonal autoregressive integrated moving average ([SARIMAX](https://www.statsmodels.org/dev/generated/statsmodels.tsa.statespace.sarimax.SARIMAX.html))
