
---
description: This endpoint is used to retrieve details relating to a particular withdrawal.
---
#Get Withdrawal

### **Parameters**

`withdrawalId` - string
Used to identify a specific withdrawal.

### **Returns**
`_id` - string

`ethAddress` - string
Ethereum public address of the user.

`starkKey` - string
The Stark public key of the user.

`token` - string
The token that was withdrawn.

`amount` - number
The amount that was withdrawn.

`createdAt` - string
The date and time of the withdrawal.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getWithdrawal \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"withdrawalId": "1a2b3c"}'
```


Result

```javascript
[
  {
    "_id": "53cb6b9b4f4ddef1ad47f943",
    "ethAddress": "0x14d06788090769f669427b6aea1c0240d2321f34",
    "starkKey": "77a3b314db07c45076d11f62b6f9e748a39790441823307743cf00d6597ea43",
    "token": "USDT",
    "amount": 1000,
    "createdAt": "2020-01-29T14:13:05.898Z"
  }
]
```