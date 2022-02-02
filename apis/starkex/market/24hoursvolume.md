---
description: Request information regarding the trading volume for a specific date. The request returns the overall trading volume details for all tokens in USD as well as the trading volume per token.
---

# Trading Volume History

### **Parameters**

none

### **Returns**

`totalUSDVolume` - number
The total trade volume in terms of USD.

`tokens` - object
List of tokens.

`startDate` - string
The start date and time for the volume presented.

`endDate` - string
The end date and time for the volume presented.

`tokenAmount` - number
The trading volume for a particular token.

`USDValue` - number
The corresponding trading volume in USD for a particular token.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/r/24HoursVolume/{Year}/{Month}/{Day} \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
    "endDate": "2021-10-10T00:00:00.450Z",
    "startDate": "2021-10-09T00:00:00.450Z",
    "symbols": {
        "1INCH:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "AAVE:ETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "AAVE:USDT": {
            "USDVolume": 179.4336011,
            "lastTrade": "2021-10-09T12:15:57.801Z",
            "lastUSDPrice": 311.09,
            "tokenAmount": 0.57679
        },
        "ALN:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ANT:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BAL:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BAT:ETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BAT:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BTC:USDC": {
            "USDVolume": 2726.35,
            "lastTrade": "2021-10-09T20:01:31.165Z",
            "lastUSDPrice": 54527,
            "tokenAmount": 0.05
        },
        "BTC:USDT": {
            "USDVolume": 119.93535,
            "lastTrade": "2021-10-09T21:51:55.516Z",
            "lastUSDPrice": 54765,
            "tokenAmount": 0.00219
        },
        "CEL:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "COMP:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "DAI:ETH": {
            "USDVolume": 1079.545439384043,
            "lastTrade": "2021-10-09T13:30:59.479Z",
            "lastUSDPrice": 1.0012033359999999,
            "tokenAmount": 1075.472
        },
        "DAI:USDT": {
            "USDVolume": 136.347934310008,
            "lastTrade": "2021-10-09T12:56:47.353Z",
            "lastUSDPrice": 0.9999,
            "tokenAmount": 136.307
        },
        "DUSK:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "DVF:USDT": {
            "USDVolume": 116131.180024218,
            "lastTrade": "2021-10-09T00:58:58.668Z",
            "lastUSDPrice": 3.8992,
            "tokenAmount": 30233.1087
        },
        "ERP:USDC": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ETH:BTC": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ETH:USDC": {
            "USDVolume": 23694.683892649,
            "lastTrade": "2021-10-09T03:12:50.905Z",
            "lastUSDPrice": 3568.7,
            "tokenAmount": 6.616565
        },
        "ETH:USDT": {
            "USDVolume": 760282.504528163,
            "lastTrade": "2021-10-09T00:01:35.935Z",
            "lastUSDPrice": 3561.2,
            "tokenAmount": 211.65481872
        },
        "HEZ:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "LDO:ETH": {
            "USDVolume": 80100.31767708,
            "lastTrade": "2021-10-09T08:02:09.337Z",
            "lastUSDPrice": 3.9054352,
            "tokenAmount": 20405.6
        },
        "LINK:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "LRC:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "MATIC:USDT": {
            "USDVolume": 1346.4451,
            "lastTrade": "2021-10-09T10:41:30.424Z",
            "lastUSDPrice": 1.3451,
            "tokenAmount": 1001
        },
        "MKR:USDT": {
            "USDVolume": 1116.264699,
            "lastTrade": "2021-10-09T12:34:37.095Z",
            "lastUSDPrice": 2520.1,
            "tokenAmount": 0.44273
        },
        "MLN:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "OMG:ETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "OMG:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "PNK:ETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "PNK:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "SHIB:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "SNX:USDT": {
            "USDVolume": 5008.01901578898,
            "lastTrade": "2021-10-09T00:07:09.787Z",
            "lastUSDPrice": 9.982,
            "tokenAmount": 490.8688
        },
        "SUSHI:USDT": {
            "USDVolume": 67.31292944,
            "lastTrade": "2021-10-09T23:09:46.266Z",
            "lastUSDPrice": 10.928,
            "tokenAmount": 6.16304
        },
        "UNI:USDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "USDC:USDT": {
            "USDVolume": 16538.310787838527,
            "lastTrade": "2021-10-09T09:02:01.189Z",
            "lastUSDPrice": 0.9999,
            "tokenAmount": 16543.09460756
        },
        "YFI:USDT": {
            "USDVolume": 68.02,
            "lastTrade": "2021-10-09T19:29:43.147Z",
            "lastUSDPrice": 34010,
            "tokenAmount": 0.002
        },
        "ZRX:ETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ZRX:USDT": {
            "USDVolume": 157.37589000000003,
            "lastTrade": "2021-10-09T04:23:48.574Z",
            "lastUSDPrice": 1.0861,
            "tokenAmount": 144.9
        }
    },
    "tokens": {
        "1INCH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "AAVE": {
            "USDVolume": 179.4336011,
            "tokenAmount": 0.57679
        },
        "ALN": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ANT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BADGER": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BAL": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BAT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "BTC": {
            "USDVolume": 2846.28535,
            "tokenAmount": 0.05219
        },
        "CEL": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "COMP": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "CRV": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "CUSDT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "DAI": {
            "USDVolume": 1215.893373694051,
            "tokenAmount": 1211.779
        },
        "DPI": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "DUSK": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "DVF": {
            "USDVolume": 116131.180024218,
            "tokenAmount": 30233.1087
        },
        "ERP": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ETH": {
            "USDVolume": 865157.051537276,
            "tokenAmount": 240.9200023597273
        },
        "EXRD": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "FUN": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "GRT": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "HEZ": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "INV": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "LDO": {
            "USDVolume": 80100.31767708,
            "tokenAmount": 20405.6
        },
        "LINK": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "LRC": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "MATIC": {
            "USDVolume": 1346.4451,
            "tokenAmount": 1001
        },
        "MKR": {
            "USDVolume": 1116.264699,
            "tokenAmount": 0.44273
        },
        "MLN": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "NEC": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "NU": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "OMG": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "PNK": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "REN": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "ROOK": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "RUNE": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "SHIB": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "SNX": {
            "USDVolume": 5008.01901578898,
            "tokenAmount": 490.8688
        },
        "SUSHI": {
            "USDVolume": 67.31292944,
            "tokenAmount": 6.16304
        },
        "TORN": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "UNI": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "USDC": {
            "USDVolume": 42959.34468048753,
            "tokenAmount": 42964.128500209
        },
        "USDT": {
            "USDVolume": 901151.1498598586,
            "tokenAmount": 901151.1498598586
        },
        "WSTETH": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "YFI": {
            "USDVolume": 68.02,
            "tokenAmount": 0.002
        },
        "ZRX": {
            "USDVolume": 157.37589000000003,
            "tokenAmount": 144.9
        },
        "wXNM": {
            "USDVolume": 0,
            "tokenAmount": 0
        },
        "xDVF": {
            "USDVolume": 0,
            "tokenAmount": 0
        }
    },
    "totalUSDVolume": 1008752.0468689715
}
```