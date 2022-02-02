---
description: Submit a request for internal transfer.
---
# Transfer

### **Parameters**

`tx` - object
StarkWare TransferRequest for main transfer

    `type` - string
    
    `amount` - string
    
    `expirationTimestamp` - integer
    
    `nonce` - integer
    
    `receiverPublicKey` - string
    
    `receiverVaultId` - integer
    
    `senderPublicKey` - string
    
    `senderVaultId` - integer
    
    `signature` - object
    
    `r` - string
    
    `s` - string
    
    `token` - string

`feeTx` - object
StarkWare TansferRequest for service fee

    `type` - string
    
    `amount` - string
    
    `expirationTimestamp` - integer
    
    `nonce` - integer
    
    `receiverPublicKey` - string
    
    `receiverVaultId` - integer
    
    `senderPublicKey` - string
    
    `senderVaultId` - integer
    
    `signature` - object
    
        `r` - string
        
        `s` - string
    
    `token` - string

`starkPublicKey` - object
The Stark public key. Both the "x" and "y" part are required.

    `x` - string
    The "x" part of the Stark public key.
    
    `y` - string
    The "y" part of the Stark public key.

`memo` - string
Optional memo string

`partnerId` - string
Optional partner Id string

### **Returns**
`_id`  - string
Transfer ID.

`token` - string
The token that was transferred.

`amount` - string
The amount that was transferred (in quantised units).

`recipient` - string
Deversifi user id of recipient of the transfer.

`createdAt` - string
The date and time transfer request was received.

`updatedAt`  - string
The date and time transfer request was received.

`tx` - object

    `type` - string
    
    `amount` - string
    
    `expirationTimestamp` - integer
    
    `nonce` - integer
    
    `receiverPublicKey` - string
    
    `receiverVaultId` - integer
    
    `senderPublicKey` - string
    
    `senderVaultId` - integer 
    
    `signature`
    
    `token` - string

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/w/transfer \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"tx":{"amount":"50005470000","senderPublicKey":"0x06c59bf9b8b5ac1fc826b473e210108aa4ee1174118ef58e6d34214bbaa7888e","receiverPublicKey":"0x024d3b90ac06389d074bb4f331852dc0d94ed2c8a3a09fdcb2bfd89e9be9e9b6","receiverVaultId":1623227486,"senderVaultId":1623227486,"token":"0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6","type":"TransferRequest","nonce":887721649,"expirationTimestamp":887656,"signature":{"r":"0x7076fceeec1283778ba54bf595de306850848dc13a2d85a4ae6b20f7df073a3","s":"0x14837f8d9a03c462eec30977372670c6e7c3c0a34d4a1f8358ce8bb4cc4c820"}},"feeTx":{"amount":"30000","senderPublicKey":"0x06c59bf9b8b5ac1fc826b473e210108aa4ee1174118ef58e6d34214bbaa7888e","receiverPublicKey":"0x037e11c9c9817ce9f3cb31ed7f00491478a7689bb8442b9ff37596ac35f41680","receiverVaultId":982288831,"senderVaultId":1623227486,"token":"0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6","type":"TransferRequest","nonce":1729595474,"expirationTimestamp":887656,"signature":{"r":"0x45232bcb8c87d9d3e744ec269f855d887a407f1ab08d13a26005354c43a43ea","s":"0x62da4284b4fa60a9da6832e062db14a46bff1386eda6e6033eac5c83b529749"}},"starkPublicKey":{"x":"06c59bf9b8b5ac1fc826b473e210108aa4ee1174118ef58e6d34214bbaa7888e","y":"1e27fc9abf6613c2584904886669790fda4c6e289ab418c6b20ae2222e738dd"}}'
```


Result

```javascript
{
  "_id": "LCafcGC6tBH",
  "token": "USDT",
  "amount": "100",
  "recipient": "0x948cd3ad67c5f21412bfcd07a7981322f9fa01f0",
  "createdAt": "2020-01-29T14:13:05.898Z",
  "updatedAt": "2020-01-29T14:13:05.898Z",
  "tx": {
    "type": "TransferRequest",
    "amount": "100",
    "expirationTimestamp": 456890,
    "nonce": 120,
    "receiverPublicKey": "0x341E46a49F15785373edE443Df0220DEa6a41Bbc",
    "receiverVaultId": 15678,
    "senderPublicKey": "0x341E46a49F15785373edE443Df0220DEa6a41Bbc",
    "senderVaultId": 1234,
    "signature": {
      "r": "5d14357fcf8f489218de0855267c6f64bc463135debf62680ad796e63cd6d3b",
      "s": "786ab874d91e3a5871134955fcb768914754760a0ada326af67f758f32819cf"
    },
    "token": "0x341E46a49F15785373edE443Df0220DEa6a41Bbc"
  }
}
```