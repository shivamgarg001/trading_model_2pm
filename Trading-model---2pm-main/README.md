# Trading-model - 3 PM
DATA is used of NSE: NIFTY 50 only  (widely used Indian Index)
Firstly, I made some data rows according to the direction and aggressiveness of momentum in the market. It is based on the positions of big players entering and exiting positions after 2 pm in INDIAN markets --> So this can lead to the aggressiveness of momentum and direction momentum.


Why 2 pm -- This is a major time when option/futures buyers and sellers are exiting their positions and making new positions for upcoming days, which results in major moves and market inefficiencies.

# Deep Learning model
I created a DL model that can tell the aggressiveness of markets at the time range of 2:00 - 3:30 (market closing) and it should be applied when a doji(indecision) candle is formed and it predicts whether a trade should be taken or not.

# How to take the trade?
Firstly, it only trained on NIFTY 50 data -- Index of Indian Stock markets, so positions should be made in options only.
Secondly, we will create a straddle whenever it tells us, whether trade should be taken or not. We will purchase ATM PE and ATM CE and wait for directional momentum.

Straddle -- First of all, it makes delta neutral and we try to play in Vega.

# Model Description
For the Deep Learning model, I have used ANN along with principal component analysis(PCA) with data cleaning and data handling techniques. For synthetic data generation and class imbalance, I used SMOTE and various techniques.










when there is momentum markets always move in one direction without disguising
So we trained the model according to binary classification and used SMOTE for data imbalance
