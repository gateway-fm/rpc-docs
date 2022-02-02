
---
description: Returns the DeversiFi application and user configuration details.
---

#Get User Config

### **Parameters**
none

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

#### **Example**

Request

```bash
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getUserConf \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" 
```


Result

```javascript
{
  "DVF": {
    "defaultFeeRate": 0.002,
    "deversifiAddress": "0x9ab450355b4ab504cbc0e4de484781dac08e6a26",
    "starkExContractAddress": "0x94E84779D79E34b9166C850c3123d42C273F8843",
    "exchangeSymbols": [
      "tETHUSD",
      "tZRXUSD",
      "tZRXETH",
      "tBTCUSD"
    ],
    "tempStarkVaultId": 1
  },
  "tokenRegistry": {
    "ETH": {
      "decimals": 18,
      "quantization": 10000000000,
      "minOrderSize": 0.05,
      "starkTokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
      "starkVaultId": 1937164364
    },
    "USDT": {
      "decimals": 6,
      "quantization": 1,
      "minOrderSize": 10,
      "settleSpread": 0,
      "starkTokenId": "0x180bef8ae3462e919489763b84dc1dc700c45a249dec4d1136814a639f2dd7b",
      "tokenAddress": "0x4c5f66596197a86fb30a2435e2ef4ddcb39342c9",
      "starkVaultId": 4937154363
    },
    "ZRX": {
      "decimals": 18,
      "quantization": 10000000000,
      "minOrderSize": 20,
      "starkTokenId": "0x3901ee6a6c5ac0f6e284f4273b961b7e9f29d25367d31d90b75820473a202f7",
      "tokenAddress": "0xcd077abedd831a3443ffbe24fb76661bbb17eb69"
    },
    "BTC": {
      "decimals": 18,
      "quantization": 10000000000,
      "minOrderSize": 0.0004,
      "starkTokenId": "0x21ef21d6b234cd669edd702dd3d1d017be888337010b950ae3679eb4194b4bc",
      "tokenAddress": "0x40d8978500bf68324a51533cd6a21e3e59be324a",
      "starkVaultId": 18264364
    }
  },
  "isRegistered": true,
  "ethAddress": "0x341e46a49f15785373ede443df0220dea6a41bbc"
}
```