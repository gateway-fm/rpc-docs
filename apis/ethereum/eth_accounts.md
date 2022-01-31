---
description: Returns a list of addresses owned by client.
---

# eth_accounts

{% hint style="warning" %}
Since Gateway does not store keys, this will always return empty.
{% endhint %}

### **Parameters**

none

### **Returns**

`Array of DATA`, 20 Bytes - addresses owned by the client.

#### **Example**

Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_accounts","params":[],"id":1}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_accounts",
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
  "result": []
}
```
