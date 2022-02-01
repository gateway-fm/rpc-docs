---
description: Returns the number of uncles in a block matching the given block hash.
---

# eth\_getUncleCountByBlockHash

### Parameters

* `DATA`, 32 Bytes - hash of a block.

```javascript
params: [
 '0xb3b20624f8f0f86eb50dd04688409e5cea4bd02d700bf6e79e9384d47d6a5a35'
]
```

### Returns

`QUANTITY` - integer of the number of uncles in this block.

### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getUncleCountByBlockHash","params":["0xb903239f8543d04b5dc1ba6579132b143087c68db1b2168786408fcbce568238"],"id":1}'
```

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": "0x1"
}
```

