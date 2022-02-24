---
description: An authenticated endpoint used to retrieve a vaultId and StarkKey
---
# Get VaultId And StarkKey

### **Parameters**
* `token` - string; The new token for which a new vault Id needs to be allocated.
* `address` - string; The Ethereum public address.

### **Returns**
* `vaultId` - number; The vault id for the requested vault.
* `starkKey` - string; The Stark public key.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/r/vaultIdAndStarkKey?token={token}&targetEthAddress={address} \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
```


Result

```javascript
{
    "vaultId": 1731798584,
    "starkKey": "0x02505c68d1a563972b3b1c6ebd9bc3556cab07be90ebd24b8fe985b88c28129c"
}