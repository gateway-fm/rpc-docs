---
description: This endpoints allows to retrieve details on all open orders.
---
# All Orders

### **Parameters**
`symbol` - string
Specifies the trading pair.

### **Returns**
`_id` - string
Id for the order. This can be used for orderId when calling cancelOrder or getOrder

`type` - string
Type of the order. Currently, "EXCHANGE LIMIT" is the only type that is supported.

`pair` - string
The trading pair that was used for this order.

`amount` - number
Actual order amount.

`totalFilled` - number
Total of all fills executed.

`price` - number
Cost per unit.

`status` - string
The status of the order.

`mtsTIF` - number
Milliseconds till order expires.

`id` - string

`created_at` - string
The date and time when the order was created.

`updated_at` - string
The date and time when the order was last updated.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/r/openOrders \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"symbol":"ETH:USD"}'
```


Result

```javascript
[
  {
    "_id": "L1tarX5wUem",
    "user": "0xc1caf2d76c49e4a60635635c329a3ac22ddeb547",
    "symbol": "ETH:USDT",
    "amount": -0.3,
    "totalFilled": -0.2,
    "price": 200,
    "averagePrice": 199.2,
    "feeRate": "0.002",
    "tokenBuy": "USDT",
    "totalBought": "4990000000",
    "tokenSell": "ETH",
    "totalSold": "45555500",
    "active": true,
    "type": "EXCHANGE LIMIT",
    "createdAt": "2020-05-09T18:29:56.882Z",
    "updatedAt": "2020-05-09T18:29:56.893Z",
    "activatedAt": "2020-05-09T18:29:56.893Z"
  },
  {
    "_id": "L1tarX5wUem",
    "user": "0xc1caf2d76c49e4a60635635c329a3ac22ddeb547",
    "symbol": "BTC:USDT",
    "amount": -0.03,
    "totalFilled": -0.01,
    "price": 8000,
    "averagePrice": 7950,
    "feeRate": "0.002",
    "tokenBuy": "USDT",
    "totalBought": "2400000000",
    "tokenSell": "BTC",
    "totalSold": "30000000",
    "active": true,
    "type": "EXCHANGE LIMIT",
    "createdAt": "2020-05-09T18:29:56.882Z",
    "updatedAt": "2020-05-09T18:29:56.893Z",
    "activatedAt": "2020-05-09T18:29:56.893Z"
  }
]

```