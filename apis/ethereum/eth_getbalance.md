---
description: Returns the balance of the account of a given address.
---

# eth\_getBalance

### Parameters

* `DATA`, 20 Bytes - address to check for balance.
* `QUANTITY|TAG` - integer block number, or the string `"latest"`, `"earliest"` or `"pending"`, see the [default block parameter](https://eth.wiki/json-rpc/API#the-default-block-parameter).

```javascript
params: [
   '0xc94770007dda54cF92009BFF0dE90c06F603a09f',
   'latest'
]
```

### Returns

`QUANTITY` - integer of the current balance for the given address in wei.


Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 89, "jsonrpc": "2.0", "method": "eth_getBalance", "params": ["0x3f5CE5FBFe3E9af3971dD833D26bA9b5C936f0bE","0x14036008"]}'
```


Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 89,
  "result": "0x1f250f59c12e1b2e"
}
```

