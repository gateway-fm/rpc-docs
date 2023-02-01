---
description: Returns all access keys for a given account.
---

# View access key list

### **Parameters**

- `method:` query
- `params:`
  - `request_type:` view_access_key_list
  - `finality` OR `block_id`
  - `account_id:` string, account id

### **Returns**

Returns all access keys for a given account.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v4/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "dontcare",
  "method": "query",
  "params": {
    "request_type": "view_access_key_list",
    "finality": "final",
    "account_id": "lunanova2.pool.f863973.m0"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "block_hash": "ihp37SupGXf6bKeiQY67174XxL1HXK5kbAbAfBh4sUR",
        "block_height": 62879969,
        "keys": []
    }
}
```
