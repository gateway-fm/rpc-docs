---
description: This is an authenticated endpoint used to retrieve deposits. A token can be specified to get deposits for a specific token. The limit of deposits returned is 1000.
---
# Deposit History

### **Parameters**

`token` - string

### **Returns**
`ethAddress` - string; The ethereum public address of the user.

`starkKey` - string; The Stark public key.

`starkVaultId` - number; The Stark vault ID.

`starkTokenId` - string; The Stark token ID.

`token` - string; The token that was deposited

`amount` - number; The amount that was deposited.

`createdAt` - string; The date and time of the deposit.

`isPostedOffchain` - boolean; Flag to indicate if the deposit was posted off chain.

`isConfirmedOnChain` - boolean; Flag to indicate if the deposit was confirmed off chain.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/getDeposits \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH"}'
```


Result

```javascript
[
    {
        "_id": "5qeXDA5Wwny",
        "pending": false,
        "token": "ETH",
        "amount": "1200000",
        "createdAt": "2021-12-23T14:03:59.870Z",
        "status": "ready"
    },
    {
        "_id": "EQxxFgA54f3",
        "pending": false,
        "token": "ETH",
        "amount": "2000000",
        "createdAt": "2021-12-23T14:02:45.020Z",
        "status": "ready"
    }
]
```
