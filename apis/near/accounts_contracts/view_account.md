---
description: Returns basic account information
---

# View account

### **Parameters**

* `method:` query
* `params:`
  * `request_type:` view_account
  * `finality` OR `block_id`
  * `account_id:` string, account id

### **Returns**

Returns basic account information

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
  "method": "query",
  "params": {
    "request_type": "view_account",
    "finality": "final",
    "account_id": "baziliknear.poolv1.near"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "amount": "39207950918041511384302365807",
        "block_hash": "3Ky29RGiqudAY19SaABBLfvZQsXrLdMBsqN9GZEssAAZ",
        "block_height": 62883714,
        "code_hash": "J1arLz48fgXcGyCPVckFwLnewNH6j1uw79thsvwqGYTY",
        "locked": "2993267216188527233791444838403",
        "storage_paid_at": 0,
        "storage_usage": 364952
    }
}
```