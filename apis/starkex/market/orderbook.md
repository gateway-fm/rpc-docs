---
description: This public endpoint allows to keep track of the state of orderbooks on a price aggregated basis with customizable precision.
---

# Orderbook

### **Parameters**

`symbol` - string
Specifies the trading pair.

`precision` - string
Set the price aggregation level. Adjust the precision by entering a value between P0-P4. Use one of the following values - P0, P1, P2, P3, P4.

`length` - string
Set the orderbook length. Adjust the max number of orders to be returned for each side by choosing between either 25 or 250.


`###` **Returns**

`Price` - number
Specifies the price level for trading.

`Count` - number
Number of orders at that price level.

`Amount` - number
Total amount available at that price level.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/market-data/book/ETH:USDT/P0/25 \
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
    302,
    1,
    20
  ],
  [
    168.02,
    1,
    0.6
  ],
  [
    167.98,
    1,
    0.6
  ],
  [
    167.94,
    1,
    0.6
  ]
]
```