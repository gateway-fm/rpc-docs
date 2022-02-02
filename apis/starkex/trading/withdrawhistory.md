---
description: An authenticated endpoint used to retrieve a list of user's past withdrawals. This includes ready, completed, as well as cancelled withdrawals. The limit of withdrawals returned is 1000.
---
# Withdrawal History

### **Parameters**

`token` - string
The token that will be withdrawn.

### **Returns**
`_id` - string
Withdrawal ID.

`token` - string
The token that was withdrawn.

`amount` - number
The amount that was withdrawn.

`createdAt` - string
The date and time of the withdrawal.

`readyToWithdrawOnChain` - bool
The withdrawal is ready to be requested.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/r/withdrawHistory \
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
    "_id": "5e318fc4948cc789bb5f7bb4",
    "token": "ETH",
    "amount": 100,
    "createdAt": "2020-01-29T14:13:05.898Z",
    "readyToWithdrawOnChain": false
  },
  {
    "_id": "5e318fc4948cc789bb5f7bb5",
    "token": "USD",
    "amount": 27,
    "createdAt": "2020-01-30T14:13:05.898Z",
    "readyToWithdrawOnChain": true
  }
]
```