---
description: >-
  Creates a filter object, based on filter options, to notify when the state
  changes (logs).
---

# eth_newFilter

Unlike `eth_newBlockFilter`which notifies you of **all **new** **blocks, you can pass in filter options to track new logs matching the topics specified. ** **


### **Parameters**

* `Object` - The filter options:
  * `fromBlock`: `QUANTITY|TAG` - (optional, default: `"latest"`) Integer block number, or `"latest"` for the last mined block or `"pending"`, `"earliest"` for not yet mined transactions.
  * `toBlock`: `QUANTITY|TAG` - (optional, default: `"latest"`) Integer block number, or `"latest"` for the last mined block or `"pending"`, `"earliest"` for not yet mined transactions.
  * `address`: `DATA|Array`, 20 Bytes - (optional) Contract address or a list of addresses from which logs should originate.
  * `topics`: `Array of DATA`, - (optional) Array of 32 Bytes `DATA` topics. Topics are order-dependent. Each topic can also be an array of DATA with “or” options.

### **Returns**

`QUANTITY` - A filter id.

### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_newFilter","params":[{"fromBlock": "0x1","toBlock": "0x2","address": "0x8888f1f195afa192cfee860698584c030f4c9db1","topics": ["0x000000000000000000000000a94f5374fce5edbc8e2a8697c15331677e6ebf0b", null, ["0x000000000000000000000000a94f5374fce5edbc8e2a8697c15331677e6ebf0b", "0x0000000000000000000000000aff3454fce5edbc8cca8697c15331677e6ebccc"]]}],"id":0}'
```

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": "0xdcc9a819f80efa9e1d215a9d41b2d22e"
}
```
