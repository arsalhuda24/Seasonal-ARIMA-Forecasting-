# Seasonal-ARIMA-Forecasting-

An important concept in time series is stationarity which states that properties of time series do not depend at the time at which the series was observed. Any time series which has a specific trend and seasonality is termed as non-stationary. Therefore it is an essential practice to make a time series stationary by removing trend and seasonality and we usually do this by differencing the time series i-e by subtracting the lagged version of ts from original series. Transformation of time series also helps to reduce the variance. 
ARIMA stands for Auto regressive moving integrated average. It is basically an ensemble of AR and MA processes
## AR(p)
Generally an autoregressive (AR) model can be represented as follows: 
y_t=c+ α_1 y_(t-1)+α_2 y_(t-2)+⋯+ α_n y_(t-n)+ Ω_t
Where Ω_t is white noise. Notice the difference with linear regression, here predictors are lagged version of time series. The above equation is referred as AR (p) model. 
For Moving average model instead of past values, past forecasted errors are modeled.
Ω_t=c+ µ_1 Ω_(t-1)+µ_2 Ω_(t-2)+⋯+ µ_p Ω_(t-p)
This is referred as MA (q) model. 
The I in ARIMA stand for the order of differencing if we combine the AR, MA and order of differencing we get ARIMA model which can be written as:
y_t=c+ α_1 y_(t-1)+α_2 y_(t-2)+⋯+ α_n y_(t-n)+µ_1 Ω_(t-1)+µ_2 Ω_(t-2)+⋯+ µ_p Ω_(t-p)  〖+Ω〗_t
We call this ARIMA (p, q, d). 
