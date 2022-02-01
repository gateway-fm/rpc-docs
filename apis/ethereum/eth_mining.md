---
description: Returns true if client is actively mining new blocks.
---

# eth_mining

#### **Parameters**

none

#### **Returns**

Boolean - returns `TRUE` of the client is mining, otherwise `FALSE`.

#### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 71, "jsonrpc": "2.0", "method": "eth_mining", "params": []}'
```
Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": false
}
```

###