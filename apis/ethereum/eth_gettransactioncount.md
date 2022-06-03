---
description: Returns the number of transactions sent from an address.
---

# eth\_getTransactionCount

### Parameters

* `DATA`, 20 Bytes - address.
* `QUANTITY|TAG` - integer block number, or the string "latest", "earliest" or "pending", see the [default block parameter](https://eth.wiki/json-rpc/API#the-default-block-parameter).

### Returns

`QUANTITY` - integer of the number of transactions send from this address.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/ethereum/archival/mainnet  \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getTransactionCount","params":["0xEA674fdDe714fd979de3EdF0F56AA9716B898ec8","latest"],"id":13}'
```


Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 13,
    "result": "0x26738a9"
}
```

