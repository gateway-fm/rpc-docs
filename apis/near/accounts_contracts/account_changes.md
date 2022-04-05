---
description: Returns account changes from transactions in a given account.
---

# View access key changes (single)

### **Parameters**
* `method:` EXPERIMENTAL_changes
* `params:`
  * `changes_type`: account_changes
  * `account_ids`: array, ["account_id"]
  * `finality` OR `block_id`
  
### **Returns**
Returns account changes from transactions in a given account.

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
    "changes_type": "account_changes",
    "account_ids": ["baziliknear.poolv1.near"],
    "finality": "final"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "block_hash": "FrcV4XbxetVixMP6Hakc9zDrB9y2837f9t8duKz5VddJ",
        "changes": []
    }
}
```