---
description: Returns individual access key changes in a specific block.
---

# View access key changes (single)

### **Parameters**

* `method:` EXPERIMENTAL_changes
* `params:`
  * `changes_type`: single_access_key_changes
  * `keys`: array, [{ account_id, public_key }]
  * `finality` OR `block_id`

### **Returns**

Returns individual access key changes in a specific block. You can query multiple keys by passing an array of objects containing the account_id and public_key.

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
      "changes_type": "single_access_key_changes",
    "keys": [
      {
        "account_id": "serhy.testnet",
        "public_key": "ed25519:EpUzdQWypMnTAjjUTEDw91t9ETiQt8LP28aG2tED5Djm"
      }
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
        "block_hash": "9U7fitAy1SUhC9u7rW4knBqxnziAnhe9BzgJ1uvGSBk8",
        "changes": []
    }
}
```