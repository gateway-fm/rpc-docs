
---
description: This is endpoint is used to retrieve the details for a specific order using the order ID.
---
# **Order**

### **Parameters**
`orderId` - string
The ID of the order. In case you want to view all open orders, check POST openOrders.

`cid` - string
An optional user-defined identifier for this order

### **Returns**
`_id` - string
Id for the order. This can be used for orderId when calling cancelOrder or getOrder

`amount` - number
Actual order amount.

`price` - number
Cost per unit.

`symbol` - string
Trading symbol for the order

`canceled` - string
Canceled status true or false.

`pending` - string
Pending status true or false.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getOrder \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"orderId": "111", "cid": "some-order-2083236893"}'
```


Result

```javascript
{
    "_id": "QrPujXPVQBY",
    "symbol": "ETH:USDT",
    "amount": -0.8,
    "price": 281,
    "totalFilled": 0,
    "pending": false,
    "canceled": false,
    "active": true
  }
```