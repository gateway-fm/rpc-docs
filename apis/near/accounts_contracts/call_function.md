---
description: Allows you to call a contract method as a view function.
---

# Call a contract function

### **Parameters**
* `method:` query
* `params:`
  * `request_type:` call_function
  * `finality` OR `block_id`
  * `account_id:` string, account id 
  * `method_name`: name_of_a_example.testnet_method 
  * `args_base64`: method_arguments_base_64_encoded

### **Returns**
Allows you to call a contract method as a view function.


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
    "request_type": "call_function",
    "finality": "final",
    "account_id": "dev-1588039999690",
    "method_name": "get_num",
    "args_base64": "e30="
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "block_hash": "2V6heaL9R3j12gACwzBm9Qsuk4L82sTkH8SV5VrvWUhE",
        "block_height": 86796995,
        "logs": [],
        "result": [
            48
        ]
    }
}
```