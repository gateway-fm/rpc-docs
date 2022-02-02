
---
description: This is an authenticated endpoint used to retrieve deposits. A token can be specified to get deposits for a specific token. The limit of deposits returned is 1000.
---
#Deposit History

### **Parameters**

`token` - string

### **Returns**
`ethAddress` - string
The ethereum public address of the user.

`starkKey` - string
The Stark public key.

`starkVaultId` - number
The Stark vault ID.

`starkTokenId` - string
The Stark token ID.

`token` - string
The token that was deposited

`amount` - number
The amount that was deposited.

`createdAt` - string
The date and time of the deposit.

`isPostedOffchain` - boolean
Flag to indicate if the deposit was posted off chain.

`isConfirmedOnChain` - boolean
Flag to indicate if the deposit was confirmed off chain.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getDeposits \
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
    "ethAddress": "0x341E46a49F15785373edE443Df0220DEa6a41Bbc",
    "starkKey": "77a3b314db07c45076d11f62b6f9e748a39790441823307743cf00d6597ea43",
    "starkVaultId": 123,
    "starkTokenId": "0x7",
    "token": "USDT",
    "amount": 1000,
    "createdAt": "2020-01-29T14:02:08.477Z",
    "isPostedOffchain": false,
    "isConfirmedOnChain": true
  }
```