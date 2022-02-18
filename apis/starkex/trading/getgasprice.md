---
description: Returns a range of gas prices in Wei to use with on chain transactions.
---
# Get Gas Price

### **Parameters**
none

### **Returns**
`fast` - number; Gas price in Wei for quickest onchain transaction confirmation.

`average` - number; Average gas price in Wei for average onchain transaction speed.

`cheap` - number; Low gas price in Wei and very slow transaction speed.

`fastWait` - number; The approximate time for a transaction confirmation when using fast as the gas price.

`averageWait` - number; The approximate time for a transaction confirmation when using average as the gas price.

`cheapWait` - number; The approximate time for a transaction confirmation when using cheap as the gas price.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/getGasPrice \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" 
```


Result

```javascript
{
    "fast": "94000000000",
    "fastWait": 0.75,
    "average": "93000000000",
    "averageWait": 3.25,
    "cheap": "92000000000",
    "cheapWait": 10.25
}
```
