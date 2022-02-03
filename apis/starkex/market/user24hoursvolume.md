---
description: Request information regarding the trading volume of a specific address for the last 24 hours. The request returns the overall trading volume details for all tokens in USD as well as the trading volume per token. Results are cached for 2 minutes.
---

# User User 24-hours volume

### **Parameters**

none

### **Returns**

`totalUSDVolume` - number
The total trade volume in terms of USD.

`tokens` - object
List of tokens.

`tokenAmount` - number
The trading volume for a particular token.

`USDValue` - number
The corresponding trading volume in USD for a particular token.


#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/User24HoursVolume \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
  "totalUSDVolume": 73364.1749445,
  "tokens": {
    "USD": {
      "tokenAmount": 85112.899879,
      "USDValue": 85112.899879
    },
    "ETH": {
      "tokenAmount": 443.61218170251453,
      "USDValue": 61525.002289
    }
  }
}
```