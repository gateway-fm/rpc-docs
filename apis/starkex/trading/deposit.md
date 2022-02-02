---
description: Submit a signed notification of a new deposit made.
---
# New Deposit

### **Parameters**

`token` - string
The token for which the deposit was made.

`amount` - number
The deposit amount.

`starkPublicKey` - object
The Stark public key. Both the "x" and "y" part are required.

    `x`- string
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

### **Returns**
`isPostedOffchain` - boolean
Flag to indicate if the deposit was posted off chain.

`isConfirmedOnChain` - boolean
Flag to indicate if the deposit was confirmed off chain.

`_id` - string

`starkVaultId` - number
The Stark vault ID.

`starkKey` - string
The Stark public key.

`starkMessage` - string
Stark Message ID.

`starkSignature`

`starkTokenId` - string
The Stark token ID.

`amount` - number
The amount that was deposited.

`ethAddress` - string
Ethereum public address of the user.

`createdAt` - string
The date and time of the deposit.

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/w/deposit \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"token":"ETH",
     "amount": 1,
     "starkPublicKey": {
        "x": "6d840e6d0ecfcbcfa83c0f704439e16c69383d93f51427feb9a4f2d21fbe075",
        "y": "58f7ce5eb6eb5bd24f70394622b1f4d2c54ebca317a3e61bf9f349dccf166cf"
      },
      "starkSignature": {
        "r": "1f38f551d798562c16d28733c7e3ff6850898d82f0ac9ccd39d373303b1778c",
        "s": "518560420e52a37e9f580f024fc0fe8572cb2f5437a839075bbf4b2b123d572",
        "recoveryParam": 1
      },
      "starkVaultId": 1000003,
      "expireTime": 1}'
```


Result

```javascript
{
  "pending": true,
  "user": "0x52d92399dfb73df49383614170880ba09b66338e",
  "token": "ETH",
  "amount": "1020400",
  "meta": {
    "ethAddress": "0x52d92399dfb73df49383614170880ba09b66338e",
    "starkKey": "00e0326547480bc8bf0fb143f08d23d3ff85aa450e6253bb721dee1410a83b73",
    "starkVaultId": 1937164364,
    "starkTokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
    "expireTime": 442425,
    "starkMessage": "598f0f08033ca8bf16552d460b2510715c689d630ef5480d50c17ada5541821",
    "starkSignature": {
      "r": "5a00d9ebdfac03fdbe55f393b34fd252447cdee79179c8c0a5227b2fe2e577",
      "s": "58e2d3972f1d482b26440197b518bb0bdeb50d03750e731118bafe3a819989d",
      "recoveryParam": 1
    },
    "nonce": 162543006
  },
  "_id": "FyqJSSXFXPU",
  "createdAt": "2020-05-22T09:43:36.348Z",
  "updatedAt": "2020-05-22T09:43:36.348Z"
}
```