---
description: Returns changes in block for given block height or hash. 

---

# Changes in Block

### **Parameters**
* `method:` EXPERIMENTAL_changes_in_block
* `params:`
  * `finality` OR `block_id`

### **Returns**
Returns changes in block for given block height or hash. You can also use finality param to return latest block details.

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
  "method": "EXPERIMENTAL_changes_in_block",
  "params": {
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
        "block_hash": "C4inBppoZQfjRvAHZqL3JBfzkGeejifhT9Y9H5KLeThH",
        "changes": [
            {
                "account_id": "bbbbbbbbbbb.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "kresko-test.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "oracle-1.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "owo.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "relay.aurora",
                "type": "account_touched"
            },
            {
                "account_id": "signer.goerli.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "zavodil.testnet",
                "type": "account_touched"
            },
            {
                "account_id": "bbbbbbbbbbb.testnet",
                "type": "access_key_touched"
            },
            {
                "account_id": "oracle-1.testnet",
                "type": "access_key_touched"
            },
            {
                "account_id": "owo.testnet",
                "type": "access_key_touched"
            },
            {
                "account_id": "relay.aurora",
                "type": "access_key_touched"
            },
            {
                "account_id": "relay.aurora",
                "type": "access_key_touched"
            },
            {
                "account_id": "relay.aurora",
                "type": "access_key_touched"
            },
            {
                "account_id": "zavodil.testnet",
                "type": "access_key_touched"
            }
        ]
    }
}
```