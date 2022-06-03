---
description: Returns the number of transactions in a block matching the given block hash.
---

# eth\_getBlockTransactionCountByHash

### Parameters

`DATA`, 32 Bytes - hash of a block.

### Returns

`QUANTITY` - integer of the number of transactions in this block.

### **Example**
Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/archival/mainnet  \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getBlockTransactionCountByHash","params":["0x58fe2b09d4c7f44899d3b657d5e98e0913786d4db887fb57125b81d02663c4f7"],"id":1}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": "0x2c"
}
```

