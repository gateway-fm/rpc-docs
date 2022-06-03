---
description: Returns a list of addresses owned by client.
---

**The method has been deprecated**

# eth_accounts

### **Parameters**

none

### **Returns**

`Array of DATA`, 20 Bytes - addresses owned by the client.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/archival/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 89, "jsonrpc": "2.0", "method": "eth_accounts", "params": []}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 89,
    "result": null,
    "error": {
        "code": -32000,
        "message": "the method has been deprecated: eth_accounts"
    }
}
```