---
description: Returns number of peers currently connected to the client.
---

# net_peerCount

### **Parameters**

none

### **Returns**

`QUANTITY` - integer of the number of connected peers.

### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"net_peerCount","params":[],"id":71}'
```


Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "0x21"
}
```
