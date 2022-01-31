---
description: Returns the current network id.
---

# net_version

#### **Parameters**

none

#### **Returns**

`String` - The current network id.

* `"1"`: Ethereum Mainnet
* `"2"`: Morden Testnet (deprecated)
* `"3"`: Ropsten Testnet
* `"4"`: Rinkeby Testnet
* `"42"`: Kovan Testnet

#### ****[**Example**]
Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"net_version","params":[],"id":67}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"net_version",
    "params":[],
    "id":67
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
  "id":67,
  "jsonrpc": "2.0",
  "result": "3"
}
```

###
