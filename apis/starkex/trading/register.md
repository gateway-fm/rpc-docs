
---
description: This method is used to register a Stark key that corresponds to an Ethereum public address. This will return deversifi Signature or DeversiFi application and user configuration details.
---
# **Register**

### **Parameters**

`starkKey` - string
The Stark public key.

### **Returns**
`DVF` - object
This contains application configuration details to set up for deposits and trading.

    `defaultFeeRate` - number
    The default fee rate, if no volume or maker discount.

    `deversifiAddress` - string
    The address of the DeversiFi exchange.

    `starkExContractAddress` - string
    Stark deposit contract address.

    `exchangeSymbols` - string
    Currency pairs available at the DeversiFi exchange for trading

    `tempStarkVaultId` - number
    Transit Stark vault ID used for deposit privacy

`tokenRegistry` - object
Detailed information related to each available token.

`isRegistered` - string
Registration status.

`ethAddress` - string
Ethereum address.

`deFiSignature` - string
Deversifi Signature

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/w/register \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"starkKey": "6d840e6d0ecfcbcfa83c0f704439e16c69383d93f51427feb9a4f2d21fbe075"}'
```


Result

```javascript
{
  "DVF": {
    "depositExpiry": 720,
    "depositNonce": 1,
    "deversifiAddress": "0x9ab450355b4ab504cbc0e4de484781dac08e6a26",
    "starkExContractAddress": "0xF3731d0cdC9834f6F32104580bD226EF1bc1A9F9",
    "exchangeSymbols": [
      "tETHUSD",
      "tZRXUSD",
      "tZRXETH"
    ],
    "tempStarkVaultId": 1
  },
  "tokenRegistry": {
    "ETH": {
      "decimals": 18,
      "minOrderSize": 0.1,
      "starkTokenId": "0x1"
    },
    "USD": {
      "decimals": 6,
      "minOrderSize": 25,
      "settleSpread": -0.026,
      "starkTokenId": "0x2",
      "tokenAddress": "0xdac17f958d2ee523a2206206994597c13d831ec7"
    },
    "ZRX": {
      "decimals": 18,
      "minOrderSize": 40,
      "starkTokenId": "22e6d888f32dea3c6e8ba64609a314eebbe1eb704e9e9febe368b0bacb21efe",
      "tokenAddress": "0xe41d2489571d322189246dafa5ebde1f4699f498"
    }
  },
  "isRegistered": true,
  "ethAddress": "0x341e46a49f15785373ede443df0220dea6a41bbc"
}
```