---
description: Used to set a specific permission for a given user
---
# Set Public Permissions

### **Parameters**
`key` - string
The permission key to change the access for

`value` - boolean
Whether to allow public access to the endpoints driven by provided permission

### **Returns**
`balances` - boolean
is balances authorized

`tradingHistory` - boolean
is trading history authorized

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/v1/trading/r/getPublicUserPermissions \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"\
-d '{"key":"balances","value":true}' \
  
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