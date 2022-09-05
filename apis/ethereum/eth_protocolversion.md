---
description: Returns the current ethereum protocol version.
---

# eth\_protocolversion

### Parameters

none

### Returns

`String` - The current ethereum protocol version.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/non-archival/mainnet  \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_protocolVersion","params":[],"id":71}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "0x42"
}
```
