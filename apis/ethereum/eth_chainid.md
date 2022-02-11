---
description: >-
  Returns the currently configured chain ID, a value used in replay-protected
  transaction signing as introduced by EIP-155.
---

# eth\_chainId

### **Parameters**

None.

### **Returns**

`QUANTITY` - integer of the current chain ID.

### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_chainId","params":[],"id":1}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": "0x1"
}
```


