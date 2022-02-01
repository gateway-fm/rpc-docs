---
description: >-
  Creates a filter in the node, to notify when new pending transactions arrive.
  To check if the state has changed, call eth_getFilterChanges.
---

# eth_newPendingTransactionFilter

### **Parameters**

None

### **Returns**

`QUANTITY` - A filter id.

### ****[**Example**]
Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_newPendingTransactionFilter","params":[],"id":0}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://rpc.gateway.fm/v1/ethereum/mainnet
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_newPendingTransactionFilter",
    "params":[],
    "id":73
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
  "jsonrpc": "2.0",
  "id": 0,
  "result": "0xa08914f1caedfcbe814d9fb33e69678d"
}
```

###
