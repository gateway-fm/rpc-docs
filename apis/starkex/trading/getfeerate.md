---
description: Return current fee rate for a given address. This rate is dependent on the trading volume of the user.
---
# Get Fee Rate

### **Parameters**

none

### **Returns**
`address` - string
The Ethereum address of the user verified by nonce and signature.

`timestamp` - number
Timestamp in milliseconds since epoch.

`fees` - object

    `maker` - number
    The fee basis points for maker orders (adding bids or offers to the order book).

    `taker` - number
    The fee basis points for taker orders (removing liquidity from the order book).

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/feeRate \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" 
```


Result

```javascript
{
  "address": "0x116f494a2ce567067f319fea1c9f294f23d2fe68",
  "timestamp": 1590263332427,
  "fees": {
    "maker": 15,
    "taker": 20
  }
}
```