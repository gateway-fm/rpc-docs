---
description: >-
  Returns a fee per gas that is an estimate of how much you can pay as a
  priority fee, or "tip", to get a transaction included in the current block.
---

# eth\_maxPriorityFeePerGas

{% hint style="danger" %}
**NOTE: **This method is not currently supported on Kovan
{% endhint %}

### Parameters

none

### **Returns**

`QUANTITY` - the estimated priority fee per gas.

#### **Example**

Request

{% tabs %}
{% tab title="Curl" %}

```bash
curl https://rpc.gateway.fm/v1/ethereum/rinkeby \
-X POST \
-H "Content-Type: application/json" \
-H "Authorization: Bearer privateKeyPart.publicKeyPart"
-d '{"jsonrpc":"2.0","method":"eth_maxPriorityFeePerGas","params":[],"id":1}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_maxPriorityFeePerGas",
    "params":[],
    "id":1
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
  "id":1,
  "jsonrpc": "2.0",
  "result": "0x12a05f1f9"
}
```
