---
description: Returns the state (key value pairs) of a contract based on the key prefix (base64 encoded). 
---

# View contract state

### **Parameters**
* `method:` query
* `params:`
  * `request_type:` view_state
  * `finality` OR `block_id`
  * `account_id:` string, account id
  * `prefix_base64`: ""
  
### **Returns**
Returns the state (key value pairs) of a contract based on the key prefix (base64 encoded). Pass an empty string for prefix_base64 if you would like to return the entire state. Please note that the returned state will be base64 encoded as well.


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
    "request_type": "view_state",
    "finality": "final",
    "account_id": "serhy.testnet",
    "prefix_base64": ""
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "block_hash": "DGBEqCgRoTipTa5sqLPdFUdvJrPyphSHqsF1t96vsRgr",
        "block_height": 86795952,
        "proof": [],
        "values": []
    }
}
```