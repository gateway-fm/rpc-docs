---
description: Request information regarding the trading volume for a specific date. The request returns the overall trading volume details for all tokens in USD as well as the trading volume per token.
---

#Trading Volume History

### **Parameters**

none

### **Returns**

`Array of DATA`, 20 Bytes - addresses owned by the client.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" 
```


Result

```javascript
{
    "jsonrpc": "2.0",
}
```