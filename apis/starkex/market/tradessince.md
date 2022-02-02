---
description: Request information regarding all completed trades in a time range for a given market pair
---

# Trades Since Date History

### **Parameters**

`Symbol` - string

`StartDate` - number
Date of the last trade returned.

`Limit` - number
Limit of trades that will be returned. With a maximum limit of 1000.

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
curl https://rpc.gateway.fm/v1/starkex/stg/v1/trading/r/tradesSince/{Symbol}/{StartDate}/{Limit} \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
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
    "timestamp": 1548028800,
    "type": "buy"
  },
  {
    "trade_id": 2,
    "price": 183.5,
    "base_volume": 1.8,
    "quote_volume": 381.28,
    "timestamp": 1558396800,
    "type": "buy"
  }
]
```
