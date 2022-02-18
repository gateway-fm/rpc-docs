---
description: An authenticated endpoint used to validate on-chain deposit  
---
# Validate deposit

### **Parameters**
`token` - string.
The token value to deposit

`amount` - string. 
Amount to deposit

### **Returns**
tokenId 
string; The tokenId value for deposit.

vaultId
string; The vault id of account for the token.

starkKey
string; The Stark public key of the user.

token
string; The token value to be deposited.

amount
string; The token amount to be deposited.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/deposits-validate \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"amount": "1000000","token": "USDT"}'
```


Result

```javascript
{
    "tokenId": "0x2ce625e94458d39dd0bf3b45a843544dd4a14b8169045a3a3d15aa564b936c5",
    "vaultId": 771611226,
    "starkKey": "0x024d3b90ac06389d074bb4f331852dc0d94ed2c8a3a09fdcb2bfd89e9be9e9b6",
    "token": "USDT",
    "amount": "1000000"
}