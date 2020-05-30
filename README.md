## Stock Market Analysis: Time Series Forecasting with ML Methods & RNN-LSTM Model

### Objective:
- To identify trends & insights from the data
- To use traditional multivariate ML methods for forecasting
- To implement RNN-LSTM algorithm to forecast the trends
- To compare the results of ML methods vis-a-vis RNN-LSTM algorithm

### About the Dataset: 
Stock Market Dataset has been obtained from Data World.
- Date Pulled: 08/29/2017 11:30pm
- Total Snapshots per Index: 2,083
- First Date Captured: September 2, 1977
- Last Date Captured: August 29, 2017

### A Brief Introduction about the Dataset:
The stock market is a large indicator of the health of the economy. Understanding the stock market, helps in predicting its trends. For this study, Nasdaq, Dow Jones, and S&P 500 market indexes are examined.

### Dow Jones Index:
The Dow Jones Industrial Average (DJIA) is a widely-watched benchmark index in the U.S. for blue-chip stocks. DJIA is a price-weighted index that tracks 30 large, publicly-owned companies trading on the New York Stock Exchange and the NASDAQ. The index was created by Charles Dow in 1896 to serve as a proxy for the broader U.S. economy.

### NASDAQ:
The Nasdaq Composite Index is a large market-cap-weighted index of more than 2,500 stocks, American depositary receipts (ADRs), and real estate investment trusts (REITs), among others.

### SP500: 
The S&P 500 Index or the Standard & Poor's 500 Index is a market-capitalization-weighted index of the 500 largest U.S. publicly traded companies. The index is widely regarded as the best gauge of large-cap U.S. equities.

### Insights From Data
The insights are found from DJIA's 30 largest publicly owned companies.
#### Top 10 Companies Based on Price
It is found that Boeing tops the chart , followed by Goldman Sachs
![Based on Price](https://user-images.githubusercontent.com/47745543/83325351-50521f80-a289-11ea-80e6-cdd7335ecb4d.JPG)

#### Companies with employees greater than or equal to 100,000
![Companies greather than = to 1 lakhs](https://user-images.githubusercontent.com/47745543/83325367-695ad080-a289-11ea-8d6c-c626a54ff6da.JPG)

#### Top 10 Companies with highest number of Employees
Walmart has the highest number of employees
![Highest Emp Top 10](https://user-images.githubusercontent.com/47745543/83325396-8c858000-a289-11ea-9c28-2dd56ce8f429.JPG)

#### Volume Analysis of Companies
Apple has the highest volume, followed by General Electric 
![Volume Analysis of Comapnies](https://user-images.githubusercontent.com/47745543/83327033-76ca8780-a296-11ea-86a9-30c0f6411a2b.JPG)

#### Top 15 Companies based on Amount
Amount here referes to Price * Volume, Apple has the highest amount followed by JPMorgan Chase
![Top 15 based on Amount](https://user-images.githubusercontent.com/47745543/83325426-bc348800-a289-11ea-8329-c56504a6fdd7.JPG)

#### Dow Jones Index over the years 
![DJ across years](https://user-images.githubusercontent.com/47745543/83325383-7b3c7380-a289-11ea-99c3-7932dae46d7a.JPG)

#### NASDAQ Index over the years
![NASDAQ values over the years](https://user-images.githubusercontent.com/47745543/83325405-9b6c3280-a289-11ea-8d38-74e343ad03f7.JPG)

#### SP500 Index over the years
![SP500 values over the years](https://user-images.githubusercontent.com/47745543/83325413-ac1ca880-a289-11ea-8a8b-f916667dced3.JPG)

#### Multivariate Time Series Forecasting:
- As part of forcasting VAR, VMA, VARMA & VARMAX were implemented 
- The Dataset was integrated to the first order to bring stationarity 
- Augumented Dickey Fuller, Granger Causality test was done to justify the approach 
- Johansen Co-integration test revealed that long term forecasting can be made with the data

#### Waveform Visualization of Data:
![VARMAX out 2](https://user-images.githubusercontent.com/47745543/83326390-47fde280-a291-11ea-9933-f16698455b46.JPG)

#### VARMAX Model Output: Prediction vs Actual
![VARMAX out 1](https://user-images.githubusercontent.com/47745543/83326395-53510e00-a291-11ea-80d8-81d524be01cd.JPG)

#### Forecasting with RNN-LSTM Model:
- Data was made stationary & was scaled to suit the RNN-LSTM model
- 70:30 was the train-test split
- With 70 units RNN-LSTM model was created

#### Loss Function Curve of RNN-LSTM Model
![LOSS CURVE RNN](https://user-images.githubusercontent.com/47745543/83326410-7380cd00-a291-11ea-9493-eb71ec31bbe0.JPG)

### Comparison Analysis
RNN-LSTM gives the best forecast, followed by VAR Model.
![Comaprison ML   RNN](https://user-images.githubusercontent.com/47745543/83326424-86939d00-a291-11ea-9458-1f1f1c534e1d.JPG)


