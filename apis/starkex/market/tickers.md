---
description: The ticker endpoint provides a high level overview of the state of the market for a specified pairs. It shows the current best bid and ask, the last traded price, as well as information on the daily volume and price movement over the last day.
---

# Tickers

### **Parameters**

`Symbol` - string
Specify the trading pair. A list of symbols can also be provided. In order to retrieve the results of all trading pairs, the symbol “ALL” should be used.

### **Returns**

`symbol` - string
The symbol of the requested trading pair.

`bid` - number
Price of the most recent highest bid.

`bid_size` - number
Sum of the 25 highest bid sizes.

`ask` - number
Price of the most recent lowest ask price.

`ask_size` - number
Sum of the 25 lowest ask sizes.

`daily_change` - number
Amount that the last price has changed since yesterday.

`daily_change_relative` - number
Relative price change since yesterday (x 100 for percentage change).

`last_price` - number
Price of the last trade.

`volume` - number
Daily volume.

`high` - number
Daily high.

`low` - number
Daily low.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/market-data/tickers?symbols=ETH:USDT \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
[
  [
    "BTC:USD",
    8719.7,
    34.58126956,
    8722.2,
    32.51991831,
    263.3,
    0.0311,
    8722.3,
    3798.87390501,
    8750,
    8449.3
  ],
  [
    "LTC:USD",
    57.875,
    1297.95111409,
    57.931,
    1670.4711322000003,
    3.233,
    0.0592,
    57.854,
    33130.37488952,
    58.18,
    54.053
  ]
]
```