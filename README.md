# Stock-Price-Estimation-Project
Estimate the stock price using machine learning

## What is our purpose?

We want to estimate the present stock price to help investor make investment decisions.

## Which stock is your choice?

We choose Apple/Microsoft/IBM(one from three) as our traget stock.

## What features are you going to take into consideration?

- Historical daily stock price (10yr)
- Historical daily S&P 500 price (10yr) as market return
- Historical Monthly 10-year U.S. treasury rate (10yr) as risk-free return
The idea comes from CAPM.

transaction costs
turnover costs

### Technical indicators:

#### Macro:
- U.S. GDP growth rate
- U.S. unemployment rate

#### Industry:
- PPI
- Companies in the same industry
- Commodity price of raw materials

#### Micro:
- P/E
- EBITDA
- EPS

#### Filter:
- Kalman filter
- Hamilton filter

### Expert reports

#### Sentiment analysis
- New York Times

## What methods do you choose?

- Decision tree
- Neutral Networks
- SVM
- ANN
- LSTM
- and more

## What is your process of project?

1. We divide the dataset into traning, validation and testing dataset, with the portion of 60%, 20%, 20%.
2. We train the model with traning dataset, tuning the hyperparameter with validation dataset and finally test the accuracy of our model with testing dataset.

## What is your traget accuracy?

Over 70% is very good. Over 80% is super good.

## How to deal with inadvertent 'cheats'?

**Yes, you cheated since you computed the signal (4pm close) to create positions (at 4pm), then you traded at 4pm. It is impossible to get these returns. Could have used Adjusted Closing at 3:55pm, then traded the closing price at 4pm.**




## DAY 1  05.01.2019
Predict stock return to be pos or neg
APPLE

One lr          : 0.5298507462686567 0.5436507936507936
500 lr AdaBoost: 0.5298507462686567 0.5436507936507936

Not Good!!!
Try to predict the target price instead of the daily return
Try to predict the monthly return and to see the accuracy

Result of Monthly return great in traning, not good in testing

One tree          : 0.6526315789473685 0.5416666666666666
500 tree AdaBoost: 0.8631578947368421 0.5416666666666666


Result from random forest   Mostly be overfitting

One tree          : 0.8947368421052632 0.6666666666666666
500 tree AdaBoost: 0.9368421052631579 0.7083333333333334

IBM
Result from random forest   Mostly be overfitting

One tree          : 0.9157894736842105 0.5
500 tree AdaBoost: 0.968421052631579 0.5


## DAY 2 05.02.2019

## Daily Target

1. Simulate stock price 
2. Plot the simulated result



## DAY 3 05.03.2019

1. Smooth the noise using kalman filter
2. Recurrent Neural Networks and Long Short-term Memory 



## DAY 4 05.04.2019

1. Add more features (Fama Fench 5-factor model)
2. Add more epoch
3. how to convert long-term variables to short-term variables







