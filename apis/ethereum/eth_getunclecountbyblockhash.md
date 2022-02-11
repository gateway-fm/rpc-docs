---
description: Returns the number of uncles in a block matching the given block hash.
---

# eth\_getUncleCountByBlockHash

### Parameters

* `DATA`, 32 Bytes - hash of a block.

### Returns

`QUANTITY` - integer of the number of uncles in this block.

### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getUncleCountByBlockHash","params":["0x09d54c053c22c07d39a9c8d0f8e6576b644b5eaa018c8180ecf541bee7bea20e"],"id":1}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": "0x0"
}
```

