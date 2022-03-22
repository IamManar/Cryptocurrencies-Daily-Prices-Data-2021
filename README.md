# Cryptocurrencies Daily Prices Data 2021
<img src="https://images.pexels.com/photos/8370752/pexels-photo-8370752.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" width="1200" height="300" alt="Cryptocurrencies Daily Prices Data 2021">

## Description 
Python script to iterate through +7600 Crypto coins to get their daily close prices in the period from 1-1-2021 to 31-12-2021 using [CryptoCompare API](https://min-api.cryptocompare.com/)
<br>
<br>
## Input
 Here's the Input I used , You can also modify your own :)


    url = "https://min-api.cryptocompare.com/data/v2/histoday"
    par = {'api_key': 'YOUR-API-KEY','fsym': fsym, 'tsym':tosym, 'limit':limit,'toTs':toTs }

- url: The API Base URL
- api_key : Obtained from the API provider 
- fsym: Coin’s symbol
- tosym: Currency that we want the pair to be converted to Default is <b>USD</b>
- limit: Number of rows we like to get default is <b>364</b>
- toTs: The timestamp we want to start from default is <b>1640908800</b>
<br>

## Output
- A Data frame in CSV format contains coins symbols as columns, Close prices as rows
- After removing empty values, we got 3369 coins prices 
<br>

## Disclaimer
- This data not fully cleaned and fully provided by [CryptoCompare API](https://min-api.cryptocompare.com/)
- Low Trade volume Coins aren't converted to USD some of them are BTC pairs and that's because conversion is done automatically when the trade volume of a certain pair is low so the system looks for a pair that has a higher volume and does the conversion which results in different prices.
