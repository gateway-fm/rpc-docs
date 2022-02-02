---
description: This returns a user ranking by overall trading volume quoted in USD. If the parameters startDate and endDate are provided, the ranking includes only trading volume within that window of time.
---

# User ranking by volume

### **Parameters**

none

### **Returns**

`address` - string
The address of the trader.

`USDValue` - number
The trading volume for the address quoted in USD.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/USDRanking \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
[
  {
    "address": "0xfc898b18a70ce49579f8d79a32e29928c15b4bc8",
    "USDValue": 119128.566703
  },
  {
    "address": "0x05e3fddf871bcba3f0651fb01fd0d621ad087be2",
    "USDValue": 32483.4076365177
  },
  {
    "address": "0x2d9e7f7887bb496592430ef62400dd9007925b88",
    "USDValue": 13434.22703491727
  }
]
```