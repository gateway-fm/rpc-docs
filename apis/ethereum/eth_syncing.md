---
description: >-
  Returns an object with data about the sync status or falseif the node is fully
  synced.
---

# eth_syncing

{% hint style="success" %}
**Note**: Your response from `eth_syncing` will likely return false because Gateway only supports nodes in production that are completed synced. 
{% endhint %}

### **Parameters**

none

### **Returns**

`Object|Boolean`, An object with sync status data or `FALSE`, when not syncing:

* `startingBlock`: `QUANTITY` - The block at which the import started (will only be reset, after the sync reached his head)
* `currentBlock`: `QUANTITY` - The current block, same as eth_blockNumber
* `highestBlock`: `QUANTITY` - The estimated highest block

### ****[**Example**]
Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_syncing","params":[],"id":1}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_syncing",
    "params":[],
    "id":1
}
```
{% endtab %}
{% endtabs %}

Response

```javascript
{
  "id":1,
  "jsonrpc": "2.0",
  "result": false
}
```
