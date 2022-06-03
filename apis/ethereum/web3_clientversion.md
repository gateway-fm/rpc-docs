---
description: Returns the current client version.
---

# web3\_clientVersion

### **Parameters**

none

### **Returns**

`String` - The current client version

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/archival/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"web3_clientVersion","params":[],"id":71}'
```


Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 71,
    "result": "erigon/2022.01.3/linux-amd64/go1.17.6"
}
```
