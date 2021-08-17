# kraken-trade-bot

This is an adaptation of [binance-trade-bot](https://github.com/edeng23/binance-trade-bot). It also leverages the [pykrakenapi](https://github.com/dominiktraxl/pykrakenapi)

## Create the keys.txt file
1. Login to [Kraken](https://www.kraken.com/u/security/api)
2. Create a new key with following permissions
    1. Funds/Query Funds
    2. Order & Trades/(all) 
    3. Other/Query Ledger Entries amd Access WebSockets API
3. In your cloned repository, create the file config/keys.txt
4. In keys.txt paste the key on line 1 and secret on line 2
5. Save

## Starting the api
```Python
import krakenex
from pykrakenapi import KrakenAPI
api = krakenex.API()
k = KrakenAPI(api)
k.api.load_key('./config/keys.txt')
```

## Available methods
You can get availaible methods by either `help(KrackenAPI)` or tab-completing `k.<tab>`.
