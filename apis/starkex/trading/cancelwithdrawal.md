
---
description: This endpoint allows to cancel a specific withdrawal with a given id.
---
#Cancel Withdrawal

### **Parameters**
`id` - string
The withdrawal ID.

### **Returns**
`_id` - string
The withdrawal ID.

`token` - string
The token for which the withdrawal was requested.

`amount` - number
The withdrawal amount.

`createdAt` - string
The date and time of the withdrawal.

`readyToWithdrawOnChain` - boolean
IF the withdrawal is ready to be requested.

`canceled` - string
Canceled status.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/w/cancelWithdrawal \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"id": "q7w8e9"}'
```


Result

```javascript
{
  "_id": "LCafcGC6tBH",
  "token": "USDT",
  "amount": "100",
  "createdAt": "2020-01-01T22:57:47.323Z",
  "readyToWithdrawOnChain": false,
  "canceled": true
}
```