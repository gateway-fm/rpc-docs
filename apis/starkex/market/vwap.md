---
description: Returns current order book snapshot of a requested pair
---

# VWAP

### **Parameters**
* `{pool}` is a valid DVF pool, like “ETH:USDT”, “DAI:ETH”, etc.
* `amount` - number; Order amount to fill positive for bid, negative for ask
* `isFirstIn` - boolean; Flag whether first symbol or second amount provided

### **Returns**
* `slippage`- number
* `estimatedPrice` - number
* `isEnoughLiquidity` - Boolean
* `executionPrice` - number

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/market-api/vwap/ETH%3AUSDT?amount=1&isFirstIn=true \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
  "estimatedPrice": 2365.068598,
  "slippage": 0.00845594452900389,
  "executionPrice": 2365,
  "isEnoughLiquidity": true
}
```
