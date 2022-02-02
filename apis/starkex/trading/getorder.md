---
description: This is endpoint is used to retrieve the details for a specific order using the order ID.
---
# Order

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
curl https://rpc.gateway.fm/v1/starkex/stg/v1/trading/r/getOrder \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"orderId": "LWwrEi9KePx"'
```


Result

```javascript
{
    "pending": false,
    "canceled": false,
    "awaitingSettlement": 0,
    "totalFilled": -0.051,
    "active": false,
    "_id": "LWwrEi9KePx",
    "symbol": "ETH:USDC",
    "amount": -0.051,
    "price": 2502.5,
    "cid": "mycid-et87a"
}
```
