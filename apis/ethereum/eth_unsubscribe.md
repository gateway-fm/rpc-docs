---
description: >-
  Subscriptions are cancelled with a regular RPC call with eth_unsubscribe as
  method and the subscription id as first parameter.
---

# eth\_unsubscribe

It returns a bool indicating if the subscription was cancelled successfully.

### Parameters

1. subscription id

### Example

{% hint style="info" %}
{% endhint %}

Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","id": 1, "method": "eth_unsubscribe", "params": ["0x9cef478923ff08bf67fde6c64013158d"]}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_subscribe",
    "params":["0x9cef478923ff08bf67fde6c64013158d"],
    "id":1
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
    "jsonrpc":"2.0",
    "id":1,
    "result":true
}
```

