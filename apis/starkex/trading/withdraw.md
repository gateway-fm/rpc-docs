---
description: Submit a request for a new withdrawal.
---
# New Withdrawal

### **Parameters**

`token` - string
The token that will be withdrawn.

### **Returns**

`token` - string
The token for which the withdrawal is requested.

`amount` - number
The withdrawal amount.

`nonce` - number
This nonce which used to provide the time until which this nonce is valid. It is presented as seconds since epoch.

`starkPublicKey` - object
The Stark public key. Both the "x" and "y" part are required.

    `x` - string
    The "x" part of the Stark public key.
    
    `y` - string
    The "y" part of the Stark public key.

`starkSignature` - object
Stark signature consisting of consisting of "r", "s" and the recovery parameter.

    `r` - string
    The "r" part of the Stark signature.
    
    `s` - string
    The "s" part of the Stark signature.
    
    `recoveryParam` - number
    The recovery parameter of the Stark signature.

`starkVaultId` - number
The Stark vault ID.

`expireTime` - number

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/stg/v1/trading/w/withdraw \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ZRX","amount":1,"nonce":1579901055.575,"starkPublicKey":{"x":"6d840e6d0ecfcbcfa83c0f704439e16c69383d93f51427feb9a4f2d21fbe075","y":"58f7ce5eb6eb5bd24f70394622b1f4d2c54ebca317a3e61bf9f349dccf166cf"},"starkSignature":{"r":"1f38f551d798562c16d28733c7e3ff6850898d82f0ac9ccd39d373303b1778c","s":"518560420e52a37e9f580f024fc0fe8572cb2f5437a839075bbf4b2b123d572","recoveryParam":1},"starkVaultId":1000003,"expireTime":442438}'
```


Result

```javascript
{
  "readyToWithdrawOnChain": false,
  "user": "0x52d92399dfb73df49383614170880ba09b66338e",
  "token": "ETH",
  "amount": "210000000",
  "meta": {
    "starkKey": "00e0326547480bc8bf0fb143f08d23d3ff85aa450e6253bb721dee1410a83b73",
    "starkVaultId": 1937164364,
    "starkTokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
    "expireTime": 442438,
    "starkMessage": "6873517319dc0130cc6910da4bb81ed4cbb800ace9ea759bb46652f0ec21093",
    "starkSignature": {
      "r": "59609e8bd25f3a434734b73a28bf581d7bfa211dc8288c235361a9833988272",
      "s": "5ea8e9bce747bc40ac9b20b38b5905cdd610d5a18145f830d97b2dbcce573a2",
      "recoveryParam": 1
    },
    "nonce": 895561747
  },
  "_id": "JUJRGVb3Wib",
  "createdAt": "2020-05-22T22:23:36.592Z",
  "updatedAt": "2020-05-22T22:23:36.592Z"
}
```
