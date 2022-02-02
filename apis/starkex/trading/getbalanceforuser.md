---
description: This is used to retrieve the total and active balances of a user per token. Active balance is the balance that is currently available. Total balance (specified as balance) is the sum of all the balances including those locked for trading.
---
# Get User Balances

### **Parameters**
`token` - string
The token which the balance is specifically requested for.

`fields` - array
Specific fields to be returned for balance information

### **Returns**
`token` - string
The token for which the balances are provided.

`balance` - number
It is the total balance for the user corresponding to the specified token.

`available` - number
It is the part of the balance available for use.

`locked` - number
It is the part of the balance currently in open orders or pending withdrawal.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getBalanceForUser/{userEthAddress} \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH","fields":["balance","updatedAt"]}'
```


Result

```javascript
[
  {
    "token": "BTC",
    "balance": 0,
    "available": 0,
    "locked": 0
  },
  {
    "token": "ETH",
    "balance": 114036369,
    "available": 89036369,
    "locked": 25000000
  },
  {
    "token": "KON",
    "balance": 99800000,
    "available": 99800000,
    "locked": 0
  },
  {
    "token": "USDT",
    "balance": 2781535529,
    "available": 2781535529,
    "locked": 0
  }
]
```