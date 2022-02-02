
---
description: Return current fee rate for a given address. This rate is dependent on the trading volume of the user.
---
#Get Fee Rate

### **Parameters**
`token` - string
The new token for which a new vault Id needs to be allocated.

### **Returns**
number 
The vault id for the requested vault.
#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getVaultId \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH"}'
```


Result

```javascript
12313567
```