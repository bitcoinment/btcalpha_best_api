![btcalpha_best_api](https://raw.github.com/bitcoinment/btcalpha_best_api/master/btcalpha_best_api.gif)

# Best API-client for Btcalpha.com

Btcalpha.com — Best API-client for Stock Exchanges (2018).
Getting fresh orders in real time.

[Check out the Interactive Demo](http://kupi.net/p/docs-api)

With this module, you can develop your own crypto-bots, analyze crypto-markets and of course, make money.

Our web-service works 24 hours and keeps high loads

The data of all exchanges come in a single format and contain extended information (links for switching to trading pairs, best asks and bids, exchange rates and much more).

---

- FREE!
- The actuality of orders is 5-30 seconds!
- Data from most exchanges
- Round-the-clock support


### Installation Instructions
    $ pip3 install btcalpha-best-api==4.0.1

### Init example
```python
from btcalpha_best_api import btcalpha_best_api
```

### Stocks API
```python
# Get all stocks
btcalpha_best_api.KUPINET('freeApi').Stocks().getList()

# Get orders by Stock name
btcalpha_best_api.KUPINET('freeApi').Stocks('Btcalpha').getOrders('ETH','BTC')

# Get all pairs from the Stock
btcalpha_best_api.KUPINET('freeApi').Stocks('Btcalpha').getAllPairs()
```
### Pairs API
```python
# Find best prices for Pair in all Stocks
btcalpha_best_api.KUPINET('freeApi').Pair('LTC','ETH').getBestPrices()
```
### Find Best Prices API
```python
# Find best ASK
btcalpha_best_api.KUPINET('freeApi').BestPrices('LTC').Ask()

# Find best BID
btcalpha_best_api.KUPINET('freeApi').BestPrices('LTC').Bid()
```
### Cryptocurrency Converter (Calculator) API
```python
# Coins list
btcalpha_best_api.KUPINET('freeApi').Calc().Data()

# Convert Coin to Coin
btcalpha_best_api.KUPINET('freeApi').Calc('LTC','ETH').Amount(10)
```

## In the future
- Unloading historical trade data
- Multi-trading through a single terminal
- Tool for crypto arbitrage
- API for JavaScript, PHP, C#
- Launch of a decentralized exchange
- Widget (calculator) for integration with sites


## About us
 We are a team of crypto developers. Our goal is to make the most convenient crypto services possible.
[Contact with us](http://kupi.net/p/support)