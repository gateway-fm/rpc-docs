---
description: >-
  Uninstalls a filter with given id. Should always be called when watch is no
  longer needed. Additionally, Filters timeout when they aren’t requested with
  eth_getFilterChangesfor a period of time.
---

# eth_uninstallFilter

### **Parameters**

`QUANTITY` - The filter id.

### **Returns**

`Boolean` - `true` if the filter was successfully uninstalled, otherwise `false`.

### ****[**Example**]
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_uninstallFilter","params":["0xfe704947a3cd3ca12541458a4321c869"],"id":0}'
```

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": false
}
```

