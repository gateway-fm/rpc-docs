
---
description: This is used to retrieve the total and active balances of a user per token. Active balance is the balance that is currently available. Total balance (specified as balance) is the sum of all the balances including those locked for trading.
---

#Balances

### **Parameters**

token

### **Returns**


#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" 
-d '{ "token": "ETH"}'
```

Result

```javascript
{
    "token":"ETH",
    "balance":"3000000",
    "available":"3000000",
    "locked":"0"}
}
```