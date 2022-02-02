---
description: Used to get all configured permissions for the authenticated user
---
# Get Public Permissions

### **Parameters**
none

### **Returns**
`balances` - boolean
is balances authorized

`tradingHistory` - boolean
is trading history authorized

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/r/getPublicUserPermissions \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
[
  {
    "balances": true,
    "tradingHistory": true
  }
]
```