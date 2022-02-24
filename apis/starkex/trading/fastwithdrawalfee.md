---
description: Return current withdrawal fee rate for a given token  
---
# Get Withdrawal Fee rate

### **Parameters**
`token` - string; Token value to get the fee

### **Returns**
* `feeBaseUnits` - number
* `feeQuantised`  - number

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/r/fastWithdrawalFee?token={token_value} \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
    "feeBaseUnits": "0.010691604",
    "feeQuantised": "1069160"
}
