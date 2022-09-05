---
description: Returns the number of transactions in a block matching the given block number.
---

# eth\_getblocktransactioncountbynumber

### Parameters

`QUANTITY|TAG` - integer of a block number, or the string "earliest", "latest" or "pending", as in the [default block parameter](https://eth.wiki/json-rpc/API#the-default-block-parameter).

### Returns

`QUANTITY` - integer of the number of transactions in this block.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/non-archival/mainnet  \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getBlockTransactionCountByNumber","params":["0x52A8CA"],"id":13}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 13,
    "result": "0x49"
}
```
