---
description: Returns a countdown until the expected next batch proof is submitted onto the blockchain and the average time of previous batches. The next batch will include all pending withdrawals.
---

# Estimated Next Batch Time

### **Parameters**

none

### **Returns**

`estimatedTime` - number
The number of seconds until the batch is sent to be processed and broadcast to the blockchain.

`averageTime` - number
The configured number of seconds between batches.

`finalisedBatchPendingConfirmation` - bool
True if the previous batch has been created but still pending confirmation on the blockchain.'

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/v1/trading/r/estimatedNextBatchTime \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
Default
[
  {
    "estimatedTime": 608,
    "token": 608,
    "finalisedBatchPendingConfirmation": true
  }
]
```
