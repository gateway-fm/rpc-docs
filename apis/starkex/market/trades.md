---
description: Request information regarding all recently completed trades for a given market pair.
---

# Trades History

### **Parameters**

`Symbol` - string

### **Returns**

`trade_id` - number
A unique ID associated with the trade for the currency pair transaction

`price` - number
Last transacted price of base currency based on given quote currency.

`base_volume` - number
Transaction amount in BASE currency.

`quote_volume` - number
Transaction amount in QUOTE currency.

`timestamp` - number
Unix timestamp in milliseconds for when the transaction occurred.

`type` - number
Used to determine whether or not the transaction originated as a buy or sell.


#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/r/trades/{Symbol} \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
[
  {
    "trade_id": 1,
    "price": 275.23,
    "base_volume": 1.5,
    "quote_volume": 347.81,
    "timestamp": 1527836800000,
    "type": "buy"
  },
  {
    "trade_id": 2,
    "price": 183.5,
    "base_volume": 1.8,
    "quote_volume": 381.28,
    "timestamp": 1577923200000,
    "type": "buy"
  }
]
```