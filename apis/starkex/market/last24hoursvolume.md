---
description: Request information regarding the trading volume for the last 24 hours. The request returns the overall trading volume details in USD as well as the trading volume per token in USD and the native token.
---

# 24hr Trading Volume

### **Parameters**

none

### **Returns**

`totalUSDVolume` - number
The total trade volume in terms of USD.

`tokens` - object
List of tokens.

`startDate` - string
The start date and time for the volume presented.

`symbols` - object
List of trading pairs.

`tokenAmount` - number
The trading volume for a particular token.

`lastUSDPrice` - number
The price in USD of the token at the most recent trade.

`USDValue` - number
The corresponding trading volume in USD for a particular token.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/last24HoursVolume \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
  "totalUSDVolume": 143437000,
  "symbols": {
    "ETH:USDT": {
      "tokenAmount": 9612.45,
      "USDVolume": 20437000,
      "lastUSDPrice": 1145.9,
      "lastTrade": "2020-05-22T16:37:37.441Z"
    },
    "BTC:USDT": {
      "tokenAmount": 12244.89,
      "USDVolume": 123000000,
      "lastUSDPrice": 10045,
      "lastTrade": "2020-05-22T16:37:37.441Z"
    }
  },
  "tokens": {
    "USDT": {
      "tokenAmount": 2956.895948,
      "USDValue": 2956.895948
    },
    "DAI": {
      "tokenAmount": 16703.14443817488,
      "USDValue": 16706.132923174882
    },
    "ETH": {
      "tokenAmount": 207.84246409836658,
      "USDValue": 34797.96540446898
    },
    "MKR": {
      "tokenAmount": 48.32582713775642,
      "USDValue": 25137.12168147688
    }
  },
  "startDate": "2020-01-19T08:09:45.342Z"
}
```
