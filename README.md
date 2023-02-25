# Backtesting-Trading-Strategies
Backtesting Trading Strategy
Asset Selection
We Should select Volatile Assets for Trading.For that we are using High to Low ratio of the assets.

((H1/L1) + (H2/L2) + ...+ (H14/L14))/14 - 1 > 3.5%

H - High,L -low , Samplesize - 14

Strategy
Assuming there is only one Standard deviation move with respect to Moving Average - Mean Reversion .

Z-score = (closeprice - rollingmovingaverage20)/(rollingstandard Deviation)

if Z-score > 1 we take short position According to Mean Reversion and we close our position when Z-Score <0

if Z-score < -1 we take long Position According to Mean Reversion and we close our position when Z-Score >0.

Platform For Backtesting
We use Quantiacs Platform for Backtesting and the time frame is Daily.

It assigns each asset Weights for Backtesting

Importing Libraries
