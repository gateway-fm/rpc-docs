---
description: This method is used to retrieve a list of all past orders for a user. This includes executed trades, as well as expired and cancelled orders. The limit of orders returned is 1000.
---
# Order History

### **Parameters**
`symbol` - string
Specifies the trading pair.

### **Returns**
`_id` - string
Order Id, this can be used as orderId when calling cancelOrder or getOrder.

`user` - string
Ethereum address of the user.

`symbol` - string
The trading pair symbol for this order.

`amount` - number
Original order size placed.

`totalFilled` - number
Total of all fills executed.

`tokenBuy` - string
Token being bought as part of this exchange order.

`totalBought` - number
Total tokens bought, in quantized units.

`tokenSell` - string
Token being sold as part of this exchange order.

`totalSold` - number
Total tokens sold, in quantized units.

`type` - string
Type of the order. Currently, "EXCHANGE LIMIT" is the only type that is supported.

`price` - number
Cost per unit.

`averagePrice` - number
Average price at which the order has been settled.

`feeRate` - number
The max fee rate applicable for the order.

`createdAt` - string
The date and time when the order was created.

`updatedAt` - string
The date and time when the order was last updated.

`activatedAt` - string
The date and time when the order was activated.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/orderHistory \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"symbol":"ETH:USDT"}'
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
