---
description: Creates a filter in the node, to notify when a new block arrives.
---

# eth_newBlockFilter

To check if the state has changed, call [`eth_getFilterChanges`](./#eth_getfilterchanges).

### **Parameters**

None

### **Returns**

`QUANTITY` - A filter id.

### ****[**Example**]
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_newBlockFilter","params":[],"id":0}'
```

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": "0x9fb7f13924bb605fd29f3ddd6d193ece"
}
```
