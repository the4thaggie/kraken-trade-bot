# kraken-trade-bot

This is an adaptation of [binance-trade-bot](https://github.com/edeng23/binance-trade-bot)
k.api.load_key('./config/keys.txt')

## Starting the api
```Python
import krakenex
from pykrakenapi import KrakenAPI
api = krakenex.API()
k = KrakenAPI(api)
k.api.load_key('./config/keys.txt')
```