---
description: An authenticated endpoint used to notify the server about incoming on-chain deposit  
---
# Notify about deposit

### **Parameters**
* `token` - string; The token value to deposit
* `amount` - string; Amount to deposit
* `txHash` - string; Transaction hash value

### **Returns**
* `pending` - Boolean
* `token` - string; Token value
* `amount` - number
* `txHash` - string; Transaction hash value
* `tx` - Object
  * `tokenId`- string
  * `vaultId` - integer
  * `starkKey` - string
  * `amount` - number
* `expiresAt` - string; The date and time
* `_id` - string
* `createdAt` - string; The date and time
* `updatedAt` - string; The date and time

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/deposits \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH","amount":400000000000000000,"txHash":"0xf6ef71a8688052915967a7f44808b232bcbe519262961ccbb903a55f6088cd83"}'
```

Result

```javascript
{
    "pending": true,
    "token": "ETH",
    "amount": "400000000000000000",
    "txHash": "0xf6ef71a8688052915967a7f44808b232bcbe519262961ccbb903a55f6088cd83",
    "tx": {
        "tokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
        "vaultId": 1623227486,
        "starkKey": "0x024d3b90ac06389d074bb4f331852dc0d94ed2c8a3a09fdcb2bfd89e9be9e9b6",
        "amount": "400000000000000000"
    },
    "expiresAt": "2022-02-19T16:51:41.264Z",
    "_id": "5o73cEU515n",
    "createdAt": "2022-02-18T16:51:41.267Z",
    "updatedAt": "2022-02-18T16:51:41.267Z"
}