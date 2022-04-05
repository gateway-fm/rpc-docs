---
description: Returns information about a single access key for given account.
---

# View access key

### **Parameters**

* `method:`query
* `params:`
  * `request_type:` view_access_key
  * `finality` OR `block_id`
  * `account_id:` string, account id
  * `public_key:` string, accound id's publick key 

### **Returns**

Returns information about a single access key for given account. If permission of the key is FunctionCall, it will return more details such as the allowance, receiver_id, and method_names.

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
  "method": "query",
  "params": {
    "request_type": "view_access_key",
    "finality": "final",
    "account_id": "serhy.testnet",
    "public_key": "ed25519:EpUzdQWypMnTAjjUTEDw91t9ETiQt8LP28aG2tED5Djm"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "block_hash": "2imUrC5YcYgY8UP9kAjNFczeW9kRGhLsdC7zVQ9AzenZ",
        "block_height": 86788151,
        "nonce": 67432542000311,
        "permission": "FullAccess"
    }
}
```