
# ETH Price Prediction Round 3 - Ocean Data Challenge

Here by my submission for Ocean Data Challenge in ETH Prediction Round 3

My approach using 24H*7Day lagged data with Fear and Greed Index for forecasting over next 24 Hours. However, only 12 Hours data were used for submission (which is the criteria for this challenge)

Here by how it's work

 1. Fetch Fear and Greed Index Data from Alternative.me
 2. Pre-processing fear and greed index
 3. Fetch Data point from Binance with ccxt
 4. Pre-processing and merge data with fear and greed index
 5. Create dataframe for training,validating and testing set

We use testing set as last 7 days for 12 hours prediction


Please visit my final report for more details

https://app.ardrive.io/#/file/f915c4e2-af28-47ed-8c17-3a58b6d3f4ee/view

Jupyter notebook are included in this repository.

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`WEB3_INFURA_PROJECT_ID`

`REMOTE_TEST_PRIVATE_KEY1` which represent your private key of your alice wallet

## Installation

To use this project you need to install following packages

```bash
# Avoid errors for the step that follows
pip install wheel

# Install Ocean library.
pip install ocean-lib

pip install predict-eth

pip install ccxt eth_account matplotlib numpy pandas prophet requests sklearn

pip install neuronprophet
```
    