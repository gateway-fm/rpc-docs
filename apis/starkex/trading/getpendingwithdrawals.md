
---
description: This endpoint is used to retrieve all pending withdrawals. If a token is specified, withdrawals pertaining to only that particular token are provided.
---

# **Pending Withdrawals**

### **Parameters**
`token` - string
The token that will be withdrawn.

### **Returns**
`ethAddress` - string
Ethereum public address of the user.

`token` - string
The token that was withdrawn.

`amount` - number
The amount that was withdrawn.

`starkKey` - string
The Stark public key of the user.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getPendingWithdrawals \
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
    "ethAddress": "0x341E46a79F25787373eaE444Df0110DEa6a4127a",
    "token": "ETH",
    "amount": 133,
    "starkKey": "1086391677682140209565436534397888993113230781145932035642834566847897455970"
  }
```