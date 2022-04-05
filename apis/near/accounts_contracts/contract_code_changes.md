---
description: Returns code changes made when deploying a contract.
---

# View contract code changes

### **Parameters**

* `method:` EXPERIMENTAL_changes
* `params:`
  * `changes_type:` contract_code_changes
  * `finality` OR `block_id`
  * `account_ids:` ["account_id"]

### **Returns**

Returns code changes made when deploying a contract. Change is returned is a base64 encoded WASM file.

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
    "changes_type": "contract_code_changes",
    "account_ids": ["pathrocknetwork.poolv1.near"],
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