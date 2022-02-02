---
description: The Candles endpoint provides OCHL (Open, Close, High, Low) and volume data for the specified funding currency or trading pair. The endpoint returns the last 100 candles by default, but a limit and a start and/or end timestamp can be specified.
---

# Candles

### **Parameters**

`key` - string
Is a group of variables defining candles key. First param currently only supports 'trade'. Second param is time frame. Available values are '1m', '5m', '15m', '30m', '1h', '3h', '6h','12h', '1D','7D', '14D', '1M'. And third is the trading pair for which information is required.

`section` - string
Section for more precise selection. Available values - "last" or "hist"


`limit` - number
Limits the number of results. Max 10000

`start` - string
Filter start (time since epoch in ms). Only when section is 'hist'

`end` - string
Filter end (time since epoch in ms). Only when section is 'hist' Defaults to now.

`sort` - number
if = 1 it sorts results returned with old > new


`###` **Returns**

`mts`  - number
Millisecond timestamp.

`open` - number
First execution during the time frame.

`close` - number
Last execution during the time frame.

`high` - number
Highest execution during the time frame.

`low` - number
Lowest execution during the time frame.

`volume` - number
Quantity of symbol traded within the time frame.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/market-data/candles/trade:1m:ETH:USDT/hist?limit=10&start=1517923200000&end=1577923200000&sort=-1 \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
[
  [
    1573562880000,
    0.0003,
    0.0003,
    0.0003,
    0.0003,
    24083.8638948
  ],
  [
    1573562820000,
    0.00030178,
    0.00033105,
    0.00033105,
    0.00030178,
    1840.0074507599998
  ]
]
```
