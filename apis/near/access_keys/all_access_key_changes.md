---
description: Returns changes to all access keys of a specific block.
---

# View access key changes (all)

### **Parameters**
* `method:` EXPERIMENTAL_changes
* `params:`
  * `changes_type`: all_access_key_changes
  * `account_ids:`: array, ["account_id_01", "account_id_02"]
  * `finality` OR `block_id`

### **Returns**
Returns changes to all access keys of a specific block. Multiple accounts can be quereied by passing an array of account_ids.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "11",
  "method": "EXPERIMENTAL_changes",
  "params": {
      "changes_type": "all_access_key_changes",
    "account_ids": [
      "serhy.testnet"
    ],
    "finality": "final"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "block_hash": "76M1NA4GXVaocZKuSU1kCwTc1K2hzXxffb6ashHM823X",
        "changes": []
    }
}
```