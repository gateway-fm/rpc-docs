---
description: Returns the application configuration details.
---
# Get Config

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

`exchangeSymbols` - array
Currency pairs available at the DeversiFi exchange for trading

`tempStarkVaultId` - number
Transit Stark vault ID used for deposit privacy

`tokenRegistry` - object
Detailed information related to each available token.

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/r/getConf \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"'
```

Result

```javascript
{
    "DVF": {
        "starkExVersion": "4",
        "defaultFeeRate": 0.002,
        "defaultFeeRateSwap": 0.003,
        "deversifiAddress": "0xc0e9bd267626e2393ddaf520ae5df27ef6c533bd",
        "deversifiAmmAddress": "0xc0e9bd267626e2393ddaf520ae5df27ef6c533bd",
        "poolAddress": "0xe64edbdc7ebdaa83e731f758825a968b84fbdaf7",
        "starkExContractAddress": "0xe73a394ade4d94a073502da8703ea23490dc7b6a",
        "starkExTransferRegistryContractAddress": "0x53AF4f40b647D5E939B1e81356883A845cc9E7b6",
        "registrationAndDepositInterfaceAddress": "0x9156F11E4005a1ED5D29f08aE1E36B2220c056dA",
        "AMMfactoryAddress": "0xc0e9bd267626e2393ddaf520ae5df27ef6c533bd",
        "AMMrouterAddress": "0xc0e9bd267626e2393ddaf520ae5df27ef6c533bd",
        "bridgeConfigPerChain": {
            "MATIC_POS": {
                "contractAddress": "0xfd54390615AEb694Ba4B63d10BE2AFbBFC5ff964",
                "withdrawalFeeRatio": 1,
                "maxWithdrawalRatio": 0.7,
                "maxTotalUsdInContract": 10000000
            }
        },
        "exchangeSymbols": [
            "ETH:USDT",
            "ZRX:USDT",
            "ZRX:ETH",
            "BTC:USDT",
            "ETH:BTC",
            "KON:RAD",
            "KON:USDT",
            "DAI:USDT",
            "DAI:ETH",
            "CUSDT:USDT",
            "ETH:USDC",
            "yvCurve-stETH:ETH",
            "DVF:USDT",
            "rDVF:DLM",
            "DVF:xDVF",
            "ERP:USDC",
            "DLM:USDC"
        ],
        "restrictedMarkets": [
            "rDVF:DLM",
            "ERP:USDC"
        ],
        "dlmMarkets": [
            "DVF:xDVF",
            "ERP:USDC"
        ],
        "tempStarkVaultId": 1,
        "minDepositUSDT": 1,
        "authVersion": 2,
        "disableLP": true,
        "deversifiStarkKeyHex": "0x003cafee3970eb7338cdd9118343f328087474ddb67aa1f572de044333a17d59"
    },
    "tokenBalancesHistory": [
        "xDVF"
    ],
    "tradingRewards": {
        "weeklyAmount": 10000,
        "rewardToken": "DVF",
        "excludedMarkets": [
            "USDC:USDT",
            "DAI:USDT"
        ]
    },
    "ammPools": {
        "DLMUSDC": {
            "tokens": [
                "DLM",
                "USDC"
            ],
            "lpToken": "LP-STG",
            "swapFees": 0.003,
            "poolFee": 0.002,
            "operatorFee": 0.001,
            "weeklyMiningReward": 20000,
            "enabled": true
        }
    },
    "tokenRegistry": {
        "ETH": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 0.05,
            "transferFee": 0.0005,
            "starkTokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0000000000000000000000000000000000000000"
            },
            "fastWithdrawalRequiredGas": 88000,
            "coingeckoId": "ethereum",
            "deployedAtBlock": 0
        },
        "DAI": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 10,
            "transferFee": 1,
            "tokenAddress": "0x633cc66389201d3884c9cc0e51eedfb0ce241e6c",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x633cc66389201d3884c9cc0e51eedfb0ce241e6c",
                "MATIC_POS": "0x0478d34dc7eb3d8622e214a3d119bd32e4a3216d",
                "MATIC_POS_PARENT": "0xaeee769968b43457589d10e4b08ee7adfe67544f"
            },
            "starkTokenId": "0x3df71c14fe878afe2df7484fdfb52b0fcec01408c590c937e872ecf607d8c51",
            "fastWithdrawalRequiredGas": 120000,
            "coingeckoId": "dai",
            "deployedAtBlock": 9681200
        },
        "USDT": {
            "decimals": 6,
            "quantization": 1,
            "minOrderSize": 10,
            "settleSpread": 0,
            "transferFee": 1,
            "starkTokenId": "0x4507594b0258664463ad7bd1d1e9b1ff67821113abd1b9c7e082bb304da322",
            "tokenAddress": "0x1c0f17436740bfb92c1070ee86322de890837c6a",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x1c0f17436740bfb92c1070ee86322de890837c6a",
                "MATIC_POS": "0x93563a298ceeba8651b81849c9f95fa314017427",
                "MATIC_POS_PARENT": "0xd997a86346e76518e6922556f34d766130c0bbfd"
            },
            "fastWithdrawalRequiredGas": 120000,
            "coingeckoId": "tether",
            "deployedAtBlock": 8051917,
            "bitfinexWithdrawalAddress": "0xc0e9bd267626e2393ddaf520ae5df27ef6c533bd"
        },
        "ZRX": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 10,
            "transferFee": 0.5,
            "starkTokenId": "0x3901ee6a6c5ac0f6e284f4273b961b7e9f29d25367d31d90b75820473a202f7",
            "tokenAddress": "0xcd077abedd831a3443ffbe24fb76661bbb17eb69",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xcd077abedd831a3443ffbe24fb76661bbb17eb69"
            },
            "fastWithdrawalRequiredGas": 120000,
            "coingeckoId": "0x",
            "deployedAtBlock": 7162114
        },
        "BTC": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 0.0004,
            "transferFee": 0.00002,
            "starkTokenId": "0x21ef21d6b234cd669edd702dd3d1d017be888337010b950ae3679eb4194b4bc",
            "tokenAddress": "0x40d8978500bf68324a51533cd6a21e3e59be324a",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x40d8978500bf68324a51533cd6a21e3e59be324a"
            },
            "fastWithdrawalRequiredGas": 120000,
            "coingeckoId": "bitcoin",
            "deployedAtBlock": 7162121
        },
        "KON": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 0.1,
            "starkTokenId": "0x167490397cac56f15cf4710f312685b9b59fb8d0a375ac17dcce5b42b4e54ae",
            "tokenAddress": "0x4024343f69875443db41f05b983aaa46c421ca75",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x4024343f69875443db41f05b983aaa46c421ca75"
            },
            "deployedAtBlock": 9151433
        },
        "RAD": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 0.1,
            "starkTokenId": "0x3df42f7fb7a67e6343d213426d9992e2cd82602b4df86a45f3f34bbfc11a973",
            "tokenAddress": "0x428a7fff5b50b7c6f8a11c75b92640327e9a5d1f",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x428a7fff5b50b7c6f8a11c75b92640327e9a5d1f"
            },
            "fastWithdrawalRequiredGas": 120000,
            "deployedAtBlock": 9151437
        },
        "CUSDT": {
            "decimals": 8,
            "quantization": 100,
            "minOrderSize": 300,
            "maxOrderSize": 10000000,
            "transferFee": 60,
            "tokenAddress": "0x622d77348301ef954d92542cf8ae106388b59c40",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x622d77348301ef954d92542cf8ae106388b59c40"
            },
            "starkTokenId": "0x20ad1647e6070723bc3a954a4af31bc2b11fe462d91ce259fb8becbf1f2bfb4",
            "coingeckoId": "compound-usdt",
            "deployedAtBlock": 9850374
        },
        "USDC": {
            "decimals": 6,
            "quantization": 1,
            "minOrderSize": 10,
            "maxOrderSize": 10000000,
            "transferFee": 1,
            "tokenAddress": "0x87f2a05b9ec0aba7f66d2c2909e2e64d9973eb71",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x87f2a05b9ec0aba7f66d2c2909e2e64d9973eb71",
                "MATIC_POS": "0xbd6d816dbb22d291c6066747693d5f6e453a3e13",
                "MATIC_POS_PARENT": "0xc09d6f77ad4a7d33d82a846493c4db38625bb3aa"
            },
            "starkTokenId": "0x177c7baa25b82a6565927ffd0322b64c672c6b3f79da010a0b798405c66caa6",
            "coingeckoId": "usd-coin",
            "deployedAtBlock": 10040002
        },
        "yvCurve-stETH": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 0.05,
            "transferFee": 0.0005,
            "tokenAddress": "0xf65c5ccfea8af44574c6f576644519c3bceda89d",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xf65c5ccfea8af44574c6f576644519c3bceda89d"
            },
            "starkTokenId": "0x1701a7f2129cadfcb853645ddc898c40e3c08b80df88dd4913bc7acdb90c9fe",
            "deployedAtBlock": 10214143
        },
        "DVF": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 1,
            "tokenAddress": "0x89c3cf486dc553225f9d3566d753a48ea03edb45",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x89c3cf486dc553225f9d3566d753a48ea03edb45"
            },
            "starkTokenId": "0x34987e656789f5fe62b1e884d30145f9d05d4eab11aad4c814255ba9f313cdc",
            "coingeckoId": "deversifi",
            "deployedAtBlock": 10296379
        },
        "rDVF": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 1,
            "tokenAddress": "0xFA604B5826246B8D23D23a21CEECE1B5434CB784",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xFA604B5826246B8D23D23a21CEECE1B5434CB784"
            },
            "starkTokenId": "0x117ab4da91b5308e9aa0234048f33e96f619b6ff36f185c2b2e42433d00024d",
            "deployedAtBlock": 10528937
        },
        "DLM": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 1,
            "tokenAddress": "0x2984890e0a345c0268D0aFB6Efe114A3A3D315B1",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x2984890e0a345c0268D0aFB6Efe114A3A3D315B1"
            },
            "starkTokenId": "0x2ff4db53dff422b8f8ed7be3407184d3dc053956fc478107cd44cfddc1d7537",
            "deployedAtBlock": 10528923
        },
        "xDVF": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 1,
            "transferFee": 1,
            "tokenAddress": "0x3aD9539C143B335794bAc9211aA5491DAEDa85Bf",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x3aD9539C143B335794bAc9211aA5491DAEDa85Bf"
            },
            "starkTokenId": "0xed35c8e6e13060ccc6a8e7cf9445cf64d9d69dc1aa5a35a5c6361700987dd2",
            "coingeckoId": "deversifi",
            "deployedAtBlock": 10296388
        },
        "ERP": {
            "decimals": 18,
            "quantization": 10000000000,
            "minOrderSize": 0.01,
            "maxOrderSize": 2500000,
            "transferFee": 1,
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0291bA2D18ea0af2DDa1D025D6C7439d811a4264"
            },
            "starkTokenId": "0x21e01fc54585d16ba65a3f38c05affa40c4d242b68e2c940c190394b3775477",
            "deployedAtBlock": 11310785
        },
        "LP-STG": {
            "decimals": 18,
            "quantization": 1000,
            "minOrderSize": 0.001,
            "maxOrderSize": 2500000,
            "transferFee": 1,
            "tokenAddressPerChain": {
                "ETHEREUM": "0x354a50252bde407efccfe4fa605498e5db68aef6"
            },
            "starkTokenId": "0x324046717bf3dabb935dc613f621e986ced6f350df325a0a691903c6fc9d68",
            "deployedAtBlock": 11519794
        }
    }
}
```
