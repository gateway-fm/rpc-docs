---
description: Returns the state change details of a contract based on the key prefix (encoded to base64).
---

# View contract state changes

### **Parameters**

* `method:` EXPERIMENTAL_changes
* `params:`
  * `changes_type:` data_changes
  * `finality` OR `block_id`
  * `account_ids:` ["account_id"]
  * `key_prefix_base64`: "base64 encoded key value"

### **Returns**

Returns the state change details of a contract based on the key prefix (encoded to base64). Pass an empty string for this param if you would like to return all state changes.

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
  "method": "EXPERIMENTAL_changes",
  "params": {
    "changes_type": "data_changes",
    "account_ids": ["pathrocknetwork.poolv1.near"],
    "key_prefix_base64": "",
    "block_id": 62888150
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "block_hash": "DwszNfJLgNkSvBa21z5LbLPrGGzp29a5muUKhREccShu",
        "changes": []
    }
}
```