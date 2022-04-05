---
description: Returns gas price for a specific block_height or block_hash.
---

# Gas Price

### **Parameters**
* `method:` gas_price
* `params:`
  * `[block_height]`, `["block_hash"]`, or `[null]`

### **Returns**
Returns gas price for a specific block_height or block_hash. Using [null] will return the most recent block's gas price.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "dontcare",
  "method": "gas_price",
  "params": [50249992]
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "gas_price": "100000000"
    }
}
```