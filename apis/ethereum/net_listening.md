---
description: Returns true if client is actively listening for network connections.

---

# net_listening

### **Parameters**

none

### **Returns**

`Boolean` - `true` when listening, otherwise `false`.

### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 89, "jsonrpc": "2.0", "method": "net_listening", "params": []}'
```

Result

```javascript
{
  "id":89,
  "jsonrpc":"2.0",
  "result":true
}
```