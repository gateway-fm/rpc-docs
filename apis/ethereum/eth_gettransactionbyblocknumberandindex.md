---
description: >-
  Returns information about a transaction by block number and transaction index
  position.
---

# eth\_getTransactionByBlockNumberAndIndex

### Parameters

* `QUANTITY|TAG` - a block number, or the string "earliest", "latest" or "pending", as in the [default block parameter](https://eth.wiki/json-rpc/API#the-default-block-parameter).
* `QUANTITY` - the transaction index position.


### Returns

See [`eth_getTransactionByHash`](./#eth_gettransactionbyhash)\`\`

### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"id": 89,"jsonrpc": "2.0","method": "eth_getTransactionByBlockNumberAndIndex","params": ["0x90f62a","0x3"]}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 89,
    "result": {
        "blockHash": "0x398bd9a4dd3a8d17940925b73b7bba8412d686ea27549dadc6311ff45e5740b8",
        "blockNumber": "0x90f62a",
        "from": "0xf5bec430576ff1b82e44ddb5a1c93f6f9d0884f3",
        "gas": "0x28b0a",
        "gasPrice": "0xba43b7400",
        "hash": "0x8c2b2666d73e4e0df8b9ad890af4974d2cf5e26dbb25822685bd7e49e86d38e3",
        "input": "0x",
        "nonce": "0x57215",
        "r": "0xa769a34b6708ac95910b1c4188c84e7a4679f1870cd6d2de54f7dc6203ea7e26",
        "s": "0x4313eca1b558e8ab8e01879105f2495bb45d5ffb55d49ef908c736d1dcab8bb",
        "to": "0x2ab0fd0338dd08a2f927a36f5a6f27b033c5eba7",
        "transactionIndex": "0x3",
        "type": "0x0",
        "v": "0x25",
        "value": "0x5decc4243fd8000"
    }
}
```

