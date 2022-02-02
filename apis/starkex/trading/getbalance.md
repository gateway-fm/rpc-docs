---
description: This is used to retrieve the total and active balances of a user per token. Active balance is the balance that is currently available. Total balance (specified as balance) is the sum of all the balances including those locked for trading.---
---
# Balances

### **Parameters**

`token` - string
The token which the balance is specifically requested for.

### **Returns**
`token` - string
The token for which the balances are provided.

`balance` - number
It is the total balance available for the user corresponding to the specified token.

`available` - number
It is the available balance for the user corresponding to the specified token.

`locked` - number

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getBalance \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH"}'
```


Result

```javascript
{
    "token":"ETH",
    "balance":"3000000",
    "available":"3000000",
    "locked":"0"
}
```