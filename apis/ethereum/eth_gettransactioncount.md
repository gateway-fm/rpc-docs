---
description: Returns the number of transactions sent from an address.
---

# eth\_getTransactionCount

### Parameters

* `DATA`, 20 Bytes - address.
* `QUANTITY|TAG` - integer block number, or the string "latest", "earliest" or "pending", see the [default block parameter](https://eth.wiki/json-rpc/API#the-default-block-parameter).

```javascript
params: [
    '0xc94770007dda54cF92009BFF0dE90c06F603a09f',
    'latest' // state at the latest block
]
```

### Returns

`QUANTITY` - integer of the number of transactions send from this address.

Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet/your-api-key \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getTransactionCount","params":["0xc94770007dda54cF92009BFF0dE90c06F603a09f","latest"],"id":0}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet/your-api-key
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_getTransactionCount",
    "params":["0xc94770007dda54cF92009BFF0dE90c06F603a09f","latest"],
    "id":0
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": "0x219"
}
```

