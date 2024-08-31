# Bitcoin-Price-Prediction
==============================

Historical Bitcoin data (01 Jan 2018 to 31 Jan 2022) was loaded using the historic_crypto library and CoinBase API, analyzed at 6-hour intervals for autocorrelation. Rolling mean and standard deviation were computed for price attributes with varying windows (3, 7, 30 days). 

The FB Prophet algorithm modeled non-stationary data, with training (2018-01-01 to 2021-08-01) and testing (2021-08-01 to 2022-01-31). FB Prophet exhibited a Mean Absolute Error of 954.50 and Root Mean Square Error of 1253.94.

Back-testing identified a strategy yielding around 2.85% by buying during 2-period price decreases and selling during 5-period increases over a month, with associated risk. 

Risk management, including Risk to Reward ratio and stop-loss mechanisms, was integrated, calculated using ATR. The framework and results were presented in a notebook.


![alt text](https://png.pngtree.com/thumb_back/fw800/background/20230715/pngtree-stock-market-surge-financial-news-bitcoin-and-plane-graph-in-3d-image_3880314.jpg)

# Generating Data:
To load the dataset, we installed the historic_crypto library which interacts with the CoinBase API to return the historical data of Bitcoin in a pandas dataframe.
We extracted the data from 01 Jan 2018 to 31 Jan 2022 for our model. We used 6-hour time interval dataset, because it preserves the autocorrelation.

# STEPS to run the project:

## STEP 01: 
Clone the repository

```bash
git clone https://github.com/Hirak010/Bitcoin-Price-Prediction.git
```

## STEP 02: 
Create an environment & activate


```bash
conda create -n env python=3.8 -y
```

## STEP 03: 
Install the requirements


```bash
pip install -r requirements.txt
```


# Authors:
```bash
Author: Biswajit Bera
Email: biswabera75@gmail.com
```
