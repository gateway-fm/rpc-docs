---
description: An authenticated endpoint used to retrieve a vaultId for given token.
---
# Get Vault Id

### **Parameters**
`token` - string
The new token for which a new vault Id needs to be allocated.

### **Returns**
number 
The vault id for the requested vault.
#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/v1/trading/r/getVaultId \
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