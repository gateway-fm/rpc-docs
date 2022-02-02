---
description: This authenticated endpoint is used to submit an order.
---
# Submit Order

### **Parameters**
`cid` - string
Optional custom order ID that could be set when placing order and used later to retrieve order. This ID is unique per user (user A and B can each have an order with cid = AAA, but the same user cannot have two orders with the same cid)

`gid` - string

`type` - string
The type of order. Currently only “EXCHANGE_LIMIT” is accepted.

`symbol` - string
The trading pair.

`amount` - number
The token amount to be traded.

`price` - number
The cost per unit.

`meta` - object
A set of meta values.

    `starkOrder` - object
    Stark order related meta information.

        `vaultIdSell` - number
        The vault ID of the seller.

        `vaultIdBuy` - number
        The vault ID of the buyer.
        
        `amountSell` - string
        The total amount to be sold.
        
        `amountBuy` - string
        The total amount to be bought.
        
        `tokenSell` - string
        The Stark token ID for the token being sold.
        
        `tokenBuy` - string
        The Stark token ID for the token being bought.
        
        `nonce` - number
        Nonce value.
        
        `expirationTimestamp` - number
        Expiration timestamp of the order.

    `starkMessage` - string
    Stark Message ID.
    
    `ethAddress` - string
    The Ethereum public address.
    
    `starkPublicKey` - object
    Detailed information related to each available token.
    
    `starkSignature`  - object
    Detailed information related to each available token.

`protocol` - string

`partnerId` - string

`feeRate` - string

### **Returns**
`_id` - string
Id for the order. This can be used for orderId when calling cancelOrder or getOrder

`user` - string
Ethereum address of the user

`symbol` - string
Trading symbol for the order

`tokenSell` - string
The token which is being sold

`tokenBuy` - string
The token which is being bought

`amount` - number
Original order size placed being sold or bought.

`price` - number
Cost per unit.

`type` - string
Type of the order. Currently, "EXCHANGE LIMIT" is the only type that is supported.

`createdAt` - string
The date and time when the order was created.

`updatedAt` - string
The date and time when the order was last updated.

`activatedAt` - string
The date and time when the order was activated.
#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/w/submitOrder \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \
-d '{"cid":"long-123","type":"EXCHANGE LIMIT","symbol":"ETH:USDT","amount":0.1,"price":1000,"meta":{"starkOrder":{"vaultIdSell":1000002,"vaultIdBuy":1000001,"amountSell":"97400000","amountBuy":"100000000000000000","tokenSell":"0x2","tokenBuy":"0x1","nonce":0,"expirationTimestamp":438947},"starkMessage":"597f31e19f2273413833ed1408edd7a2c60e9f82422852a1be7d11049be3268","ethAddress":"0x341E46a49F15785373edE443Df0220DEa6a41Bbc","starkPublicKey":{"x":"6d840e6d0ecfcbcfa83c0f704439e16c69383d93f51427feb9a4f2d21fbe075","y":"58f7ce5eb6eb5bd24f70394622b1f4d2c54ebca317a3e61bf9f349dccf166cf"},"starkSignature":{"r":"5d14357fcf8f489218de0855267c6f64bc463135debf62680ad796e63cd6d3b","s":"786ab874d91e3a5871134955fcb768914754760a0ada326af67f758f32819cf","recoveryParam":0}},"feeRate":0.1}' '
```


Result

```javascript
{
  "pending": true,
  "_id": "",
  "user": "0xc2fff68dbdb8c0dcceb2b84a921cc2c8004104fa",
  "symbol": "ZRX:ETH",
  "amount": 50,
  "type": "EXCHANGE LIMIT",
  "price": 0.005,
  "feeRate": 0.002,
  "partnerId": "P1",
  "meta": {
    "ethAddress": "0xc2fff68dbdb8c0dcceb2b84a921cc2c8004104fa",
    "starkPublicKey": {
      "x": "07fc758ce6d8591c46b34c4c94f37c81f9a2763cf7b4abce7779bfeea582a754",
      "y": "12e340b350a82322bae0106b952d5b9a3a80265dfa4228acb8c4e309bacd826"
    },
    "starkOrder": {
      "vaultIdSell": 1845686579,
      "vaultIdBuy": 1671627635,
      "amountSell": "25000000",
      "amountBuy": "4990000000",
      "tokenSell": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
      "tokenBuy": "0x3901ee6a6c5ac0f6e284f4273b961b7e9f29d25367d31d90b75820473a202f7",
      "nonce": 143600912,
      "expirationTimestamp": 442384
    },
    "starkMessage": "6157ce5d1df3572f43cfae5742454988218e4106797f0fcbe820a984215803e",
    "starkSignature": {
      "r": "34fbf0f9eab6b26388e96abfaa9903c257e64f268ab0a3246ac2bcbfc3f5154",
      "s": "4836111bf1cb0683b6145ebf667ec01030d7e25d3832f28fadb0dfcd9522b43",
      "recoveryParam": 0
    }
  },
  "tokenSell": "ETH",
  "tokenSellLockedBalance": "25000000",
  "tokenBuy": "ZRX",
  "createdAt": "2020-05-20T16:24:36.452Z",
  "updatedAt": "2020-05-20T16:24:36.452Z"
}
```
