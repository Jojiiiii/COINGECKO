# COINGECKO
CoinGecko Spreadsheet Feed: Prices, Volumes, Market Cap


######
## PUBLICATION LINKS
###### [Link to Google Sheets!](https://docs.google.com/spreadsheets/d/1-QNPo7-gq3vLMoxrCWg_DwTA5dfD9b-Lv-tRVTqo1RE/edit?usp=sharing)   
###### [Link to Youtube](https://www.youtube.com/watch?v=e73I-5FkL7E) 
###### [Link to the Medium Publication](https://medium.com/the-cryptocurious/coingecko-prices-volumes-market-caps-in-google-sheets-and-excel-a1a3ee201cb8)
###### [Link to GOOGLE SHEET SET-UP Set-up](https://medium.com/the-cryptocurious/google-sheet-open-source-cryptotools-set-up-9420e3940a8a)

## GECKOPRICE
### Imports CoinGecko's cryptocurrency prices into Google spreadsheets. 

![CoingeckoPrice](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/geckoprice_array.gif)

###### =GECKOPRICE(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOPRICE("BTC", "USD","$A$1")
##### EXAMPLE    =GECKOPRICE(A1:A10)


######

## GECKOVOLUME
### Imports CoinGecko's cryptocurrency volumes into Google spreadsheets. 

![GeckoVolumeEur](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/geckoVOLUME_array_EUR.gif)

###### =GECKOVOLUME(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOVOLUME("BTC", "USD","$A$1")
##### EXAMPLE    =GECKOVOLUME(A1:A10, "EUR")


######

## GECKOCAP
### Imports CoinGecko's cryptocurrency market capitalization into Google spreadsheets. 

![alt text](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCAP.gif)

###### =GECKOCAP(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOCAP("BTC", "USD","$A$1")
##### EXAMPLE    =GECKOCAP(A1:A10, "EUR")


######
## GECKOPRICEBYNAME
### Imports CoinGecko's cryptocurrency prices into Google spreadsheets. The Id of cryptocurrency ticker can be found in the following coingecko web page  (https://api.coingecko.com/api/v3/search?locale=fr&img_path_only=1)

![GECKOPRICEBYNAME](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOPRICEBYNAME.gif)

###### =GECKOPRICEBYNAME(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOPRICEBYNAME("bitcoinV", "USD","$A$1")

######

## GECKOATH GECKOATL
### Imports CoinGecko's cryptocurrency All Time High AND Low Prices into Google spreadsheets. 

![GECKOATHL](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/geckoathatl_array.gif)

###### =GECKOATH(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOATH("BTC", "USD","$A$1")
##### EXAMPLE    =GECKOATH(A1:A10, "EUR")

###### =GECKOATL(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKOATL("BTC", "USD","$A$1")
##### EXAMPLE    =GECKOATL(A1:A10, "EUR")

######
## GECKO24HPRICECHANGE
### Imports CoinGecko's 24h Price % change into Google spreadsheets. 

![GECKOATH](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/gecko24hpricechange_array.gif)

###### =GECKOATH(ticker,currency, refresh_cell) 
##### EXAMPLE    =GECKO24HPRICECHANGE("BTC", "USD","$A$1")
##### EXAMPLE    =GECKO24HPRICECHANGE(A1:A10, "EUR")

######
######
## GECKOCHANGE
### Imports CoinGecko's cryptocurrency price change, volume change and market cap change into Google spreadsheets. 
###### =GECKOCHANGE(ticker,type, nb_days, refresh_cell) 

### GECKO PRICE CHANGE decimal form
![GECKOCHANGEPRICE](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCHANGE2.gif)

##### EXAMPLE    =GECKOCHANGE("BTC","USD","PRICE",1,"$A$1")

### GECKO VOLUME CHANGE decimal form
![GECKOCHANGEVOL](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCHANGE2VOLUME.gif)

##### EXAMPLE    =GECKOCHANGE("BTC","USD","VOLUME",365,"$A$1")

### GECKO MARKET CAP CHANGE, decimal form
![GECKOCHANGECAP](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCHANGE2MKTCAP.gif)

##### EXAMPLE    =GECKOCHANGE("BTC","USD","MARKETCAP",365,"$A$1")

### GECKOHIST, decimal form, gets the list of historical prices, volumes, market cap
![GECKOHIST](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOHIST.gif)

##### EXAMPLE    =GECKOHIST("ethereum","usd","price",datevalue("12-31-2020"),datevalue("08-31-2020"))
Depending on the timezone of your sheet either datevalue('mm-dd-yyyy') or datevalue('dd-mm-yyyy')

### GECKOCAPTOT, gets the current total market cap of cryptocurrencies
![GECKOCAPTOT](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCAPTOT.gif)

##### EXAMPLE    =GECKOCAPTOT()

### GECKOCAPDOMINANCE, gets the % market cap dominance by cryptocurrencies
![GECKOCAPDOMINANCE](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOCAPDOMINANCE.gif)

##### EXAMPLE    =GECKOCAPDOMINANCE("BTC")

### GECKOSUPPLY gets the coin's circulating, max & total supply
### Imports the circulating supply 
![GECKOSUPPLY](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOSUPPLY.gif)
##### EXAMPLE    =GECKOSUPPLY("ETH")

### Imports the maximum supply 
![GECKOMAXSUPPLY](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOSUPPLY_MAXSUPPLY.gif)
##### EXAMPLE    =GECKOSUPPLY("BTC","MAX_SUPPLY")

### Imports the total supply 
![GECKOTOTALSUPPLY](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/GECKOSUPPLY_TOTALSUPPLY.gif)
##### EXAMPLE    =GECKOSUPPLY("BTC","TOTAL_SUPPLY")

### FORMULA REFRESHING & MAKING SURE NOT TO TRIGGER GOOGLE LIMITS
![TickerBox](https://github.com/Eloise1988/COINGECKO/blob/master/GIF/TickerBoxRefresh.gif)

##### EXAMPLE    =if($C$10=true, GECKOPRICE(B12:B32,"usd",$B$10),"Tick Box to Refresh")



