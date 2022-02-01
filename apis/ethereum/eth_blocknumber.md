---
description: Returns the number of the most recent block.
---

# eth\_blockNumber

## Parameters

none

## Returns

`QUANTITY` - integer of the current block number the client is on.

### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":71}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "0xd77735"
}
```
