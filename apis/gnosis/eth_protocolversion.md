---
description: Returns the current ethereum protocol version.
---

# eth\_protocolVersion

### Parameters

none

### Returns

`String` - The current ethereum protocol version.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_protocolVersion","params":[],"id":71}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "65"
}
```

