---
description: This method is used to retrieve a list of all past executed trades for a user. This includes the different trades that have been settled for each fully executed or partially executed order.
---
# User Trade History

### **Parameters**
none

### **Returns**
`items` - array

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/publicTradeHistory/{user} \
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
    "items": [
      {
        "fillAmount": -0.05,
        "user": "0x271f6a30fcf762325d3213ce19ed55e7e6a8cac1",
        "date": "2021-05-06T09:54:33.433Z",
        "tokenBuy": "USDT",
        "tokenSell": "ETH",
        "amountBuy": "9.985",
        "amountSell": "0.05",
        "orderId": "MSf8g3RbctU",
        "feeCurrency": "USDT",
        "feeAmount": "0.015"
      }
    ]
  }
]
```