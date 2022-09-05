---
description: Returns the current price per gas in wei.
---

# eth\_gasprice

### Parameters

none

### Returns

`QUANTITY` - integer of the current gas price in wei.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/non-archival/mainnet  \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_gasPrice","params":[],"id":71}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "0x20688d341a"
}
```
