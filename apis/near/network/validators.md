---
description: Queries active validators on the network returning details and the state of validation on the blockchain.
---

# Validation Status

### **Parameters**

* `method:` validators
* `params:`
  * `["block hash"]`, `[block number]`, or `[null]` for the latest block

### **Returns**

Queries active validators on the network returning details and the state of validation on the blockchain.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "11",
  "method": "validators",
  "params": [62909946]
}'
```

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "11",
  "method": "validators",
  "params": [null]
}'
```