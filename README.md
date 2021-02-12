# A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies. 

In this assignment, many time series tools were used to predict future movements in the value of the Canadian dollar versus the Japanese yen.

Below concepts were used to achieve the above task:

1. Time series forecasting
2. Linear regression modelling

- - -

### Files

[Time-Series Starter Notebook](Starter_Code/time_series_analysis.ipynb)

[Linear Regression Starter Notebook](Starter_Code/regression_analysis.ipynb)

[CAD/JPY Data CSV File](Starter_Code/cad_jpy.csv)

- - -

### Modelling Process

#### Time-Series Forecasting

In the time_series_analysis notebook, historical CAD-JPY exchange rate was imported, time series analysis and modelling were utlized to determine if there is any predictable behaviour.

I created time series models and forecasted the movement of the currencies using three concepts - ARMA, ARIMA and GARCH as outlined below:

1. Decomposition using a Hodrick-Prescott filter (decomposed the settle price into trend and noise).
2. Forecasted returns using an ARMA model.
3. Forecasted the exchange rate price using an ARIMA model.
4. Forecasted volatility with GARCH.

Time series analysis and modelling helped answer the following questions:

1. Based on your time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would you feel confident in using these models for trading?

#### Linear Regression Forecasting

In regression_analysis.ipynb notebook, Scikit-Learn linear regression model was built to predict CAD/JPY returns with *lagged* CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

Below steps were completed during the modelling process:

1. Data preparation (creating returns and lagged returns, and splitting the data into training and testing data)
2. Fitting a linear regression model.
3. Making predictions using the testing data.
4. Out-of-sample performance.
5. In-sample performance.

Following question was answered using the results of the linear regression analysis and modelling:

* Does this model perform better or worse on out-of-sample data compared to in-sample data?

### Glossary

* Out-of-sample data is data that the model hasn't seen before (testing data).
* In-sample data is data that the model was trained on (training data).

