---
description: This returns a user ranking by trading volume for a chosen token. If the parameters startDate and endDate are provided, the ranking includes only trading volume within that window of time. All volumes are quoted in ETH.
---

# **Volume ranking by token**

### **Parameters**

none

### **Returns**

`address` - string
The address of the trader.

`amount` - number
The trading volume for the address


#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/tokenRanking \
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
    "amount": 852.9290936325145
  },
  {
    "address": "0x05e3fddf871bcba3f0651fb01fd0d621ad087be2",
    "amount": 243.9949461819435
  },
  {
    "address": "0x2d9e7f7887bb496592430ef62400dd9007925b88",
    "amount": 100.03447614758483
  },
  {
    "address": "0x239271f50e1461ad9a4f8114b05e48f229f5c1ae",
    "amount": 0.1
  }
]
```