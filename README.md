## Time Series Forecasting of Index Funds and Crypto-based Exchange-Traded Funds
![stock-market-thumb](https://user-images.githubusercontent.com/76742936/146246147-f343f14d-8134-4655-b8cb-c5e8ef1edf32.jpg)


### Business
Start-up company Crypt wants to determine the predictability of crytpo and crypto related assets. Additionally, the company wants to compare the price action of traditional market ETFs to those following crypto. The goal of Crypt is to determine the relative maturity of crypto assets by looking at volatility and valuation forecast against traditional market institutions.

How volatile are crypto assets?
How predictable are crypto assets compared to traditional market ETFs?
How do the valuation forecasts of crypto assets perform against traditional market ETFs?


### Data
Bitwise - ETF (Tracks top ten cryptocurrency by measure of market capitalization)
SPY - ETF (Exchange-Traded Fund that tracks SP500 Index)
QQQM - ETF (Exchange-Traded Fund that tracks NASDAQ Composite Index)
DIA - ETF (Exchange-Traded Fund that tracks Dow Jones Industrial Average Index)
BLOK - Index Fund (Crypto and Blockchain Related Industries)
All datasets contain the columns 'Open', 'High', 'Low', 'Close', 'Adj Close', and 'Volume'. 'Open' and 'Close' are the prices of the ETFs taken at 9:30 AM and 4:00 PM. The 'High' and 'Low' are points during the day that marks the peak and trough of each ETF's price. The adjusted close ('Adj Close') is the price of the ETF after corporate actions which may affect valuation after accounting. DIA, SPY, and BLOK start on March 3rd, 2020. BITW starts on December 10, 2020 and QQQM starts on October 13, 2020. All data end on November 17, 2021. The rows are timestamped with the day of month only for weekdays, it does not include data from weekends and bank holidays (stock markets are closed).

### Methods
The principal method this analysis uses is time series forecasting. In order of iteration, Random Walk, Autoregression, Moving Average, ARIMA, SARIMA, and Facebook Prophet modeling are used to create predictive and forecasting models. Each model serves to inform and hone the previous model's shortcomings. Additionally, autocorrelation function (ACF), partial autocorrelation function (PACF), decomposition are used to dissect and learn optimal parameters for the models. While the Dickey-Fuller Test, Akaike Information Criterion, mean squared error, and root mean squared error are used to asses the accuracy and fit of the models.

### Results 
Dow Jones ETF

![image](https://user-images.githubusercontent.com/76742936/146247401-02805c8f-6b0f-4c77-987b-5d2dba4ccba3.png)

SP500 ETF

![image](https://user-images.githubusercontent.com/76742936/146247366-10a58ea7-9913-4b70-95e6-70b66427d5de.png)

NASDAQ ETF

![image](https://user-images.githubusercontent.com/76742936/146247452-fbcb1b3c-7df5-4140-8855-db42f0c1648e.png)

Bitwise ETF

![image](https://user-images.githubusercontent.com/76742936/146247483-3d3bad2c-2f7b-4c02-a4e3-8a4241e55b67.png)

Blok Index Fund

![image](https://user-images.githubusercontent.com/76742936/146247506-c2a76589-50de-44f5-9755-ad012ec49d89.png)

### Analysis 
As expected, the valuation of the traditional stockmarket assets were easier to predict both in terms of precission and confidence. The lower root mean squared error seen with SPDR Dow Jones Industrial Average ETF, SPDR S&P 500 ETF Trust, and Invesco NASDAQ 100 ETF are markedly lower than those of Bitwise and Blok.

As for Crypt, Bitwise and Blok assets both show immaturity in predictability and volatility. Bitwise ETF and Blok Index Fund has a short history. Both were started within the past two years as opposed to decades of history behind DIA, SPY, and QQQM. Models suffered from insufficient data surrounding Bitwise and Blok.

### Looking Ahead
data available on coins span back years before ETFs or index funds were created to track and invest in crypto-related assets. Higher volatility might be worthwhile as a trade-off for more accurate seasonality and periodicity that forecasting individual coins may give us. However, the goal of analysis would change. Instead of comparing the traditional market to an emerging crypto-based market, this new analysis would focus more on the performance of returns in investing in individual coins while using traditional market ETFs as a measuring stick. Similar to comparing Tesla's performance against DIA.

Conversely, we can wait for the crypto industry to mature further in order to make a better assessment similar to the one we attempted to make in this research. In just a few years time, ETFs and index funds like Bitwise and Blok will have more data, which would make modeling and forecasting with regardes to seasonality and periodicity improve.

