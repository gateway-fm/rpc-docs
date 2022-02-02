
---
description: Returns the application configuration details.
---
#Get Config

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
curl https://rpc.dev.gateway.fm/v1/starkex/prod/v1/trading/r/getConf \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"'
```

Result

```javascript
{
    "DVF": {
        "authVersion": 2,
        "bridgeFeesPerChain": {
            "MATIC_POS": 1
        },
        "bridgedDepositContractsPerChain": {
            "MATIC_POS": "0xBA4EEE20F434bC3908A0B18DA496348657133A7E"
        },
        "defaultFeeRate": 0.002,
        "defaultFeeRateSwap": 0.003,
        "deversifiAddress": "0xaf8ae6955d07776ab690e565ba6fbc79b8de3a5d",
        "deversifiStarkKeyHex": "0x037e11c9c9817ce9f3cb31ed7f00491478a7689bb8442b9ff37596ac35f41680",
        "dlmMarkets": [
            "DVF:xDVF"
        ],
        "exchangeSymbols": [
            "ETH:USDT",
            "MKR:USDT",
            "PNK:ETH",
            "PNK:USDT",
            "DAI:ETH",
            "DAI:USDT",
            "BTC:USDT",
            "BTC:USDC",
            "ZRX:ETH",
            "ZRX:USDT",
            "DUSK:USDT",
            "ETH:BTC",
            "USDC:USDT",
            "OMG:ETH",
            "OMG:USDT",
            "LINK:USDT",
            "BAT:USDT",
            "BAT:ETH",
            "MLN:USDT",
            "COMP:USDT",
            "UNI:USDT",
            "YFI:USDT",
            "BAL:USDT",
            "HEZ:USDT",
            "ANT:USDT",
            "SNX:USDT",
            "AAVE:USDT",
            "AAVE:ETH",
            "SUSHI:USDT",
            "LRC:USDT",
            "CUSDT:USDT",
            "LDO:ETH",
            "ALN:USDT",
            "ETH:USDC",
            "1INCH:USDT",
            "CEL:USDT",
            "DVF:USDT",
            "DVF:xDVF",
            "MATIC:USDT",
            "ERP:USDC",
            "SHIB:USDT"
        ],
        "minDepositUSDT": 1,
        "registrationAndDepositInterfaceAddress": "0xeD9d63a96c27f87B07115b56b2e3572827f21646",
        "starkExContractAddress": "0x5d22045DAcEAB03B158031eCB7D9d06Fad24609b",
        "starkExTransferRegistryContractAddress": "0xc3CA38091061e3E5358A52d74730F16C60cA9c26",
        "tempStarkVaultId": 1,
        "withdrawalBalanceReaderContractAddress": "0x650ca2dca7e2e2c8be3bb84e0a39dd77891d4d1e"
    },
    "ammPools": {
        "ETHUSDT": {
            "lpToken": "LP-ETHUSDT",
            "operatorFee": 0.001,
            "poolFee": 0.003,
            "tokens": [
                "ETH",
                "USDT"
            ]
        },
        "ETHUST": {
            "lpToken": "LP-ETHUST",
            "operatorFee": 0.002,
            "poolFee": 0.004,
            "tokens": [
                "ETH",
                "UST"
            ]
        },
        "KONDVF": {
            "lpToken": "LP-KONDVF",
            "operatorFee": 0.001,
            "poolFee": 0.003,
            "tokens": [
                "KON",
                "DVF"
            ]
        }
    },
    "tokenBalancesHistory": [
        "xDVF"
    ],
    "tokenRegistry": {
        "1INCH": {
            "coingeckoId": "1inch",
            "decimals": 18,
            "deployedAtBlock": 11511393,
            "minOrderSize": 10,
            "quantization": 10000000000,
            "starkTokenId": "0x1debe4e8d8dee240a8cfffc66847313a5d072eda164cc38733ac4a5cddca0da",
            "tokenAddress": "0x111111111117dc0aa78b770fa6a738034120c302",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x111111111117dc0aa78b770fa6a738034120c302"
            },
            "transferFee": 0.2
        },
        "AAVE": {
            "coingeckoId": "aave",
            "decimals": 18,
            "deployedAtBlock": 10926829,
            "fastWithdrawalRequiredGas": 280000,
            "maxOrderSize": 10000000,
            "minOrderSize": 0.1,
            "quantization": 10000000000,
            "starkTokenId": "0x2b018dcfca4a25c9a12c06b82af401bafa86a72c3c54ca0b58077b4b954ea33",
            "tokenAddress": "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9"
            },
            "transferFee": 0.002
        },
        "ALN": {
            "coingeckoId": "aluna",
            "decimals": 18,
            "deployedAtBlock": 11966482,
            "maxOrderSize": 10000000,
            "minOrderSize": 40,
            "quantization": 10000000000,
            "starkTokenId": "0x361ad684e3387e6c56e3faab7ad4829781716bfd9b7e6b341d9481f0019c058",
            "tokenAddress": "0x8185bc4757572da2a610f887561c32298f1a5748",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x8185bc4757572da2a610f887561c32298f1a5748"
            },
            "transferFee": 2
        },
        "ANT": {
            "coingeckoId": "aragon",
            "decimals": 18,
            "deployedAtBlock": 11060110,
            "minOrderSize": 5,
            "quantization": 10000000000,
            "starkTokenId": "0x20f290220d6ed1c1b91466f0f827e43406d182c8b7783b0df728b4f40fae233",
            "tokenAddress": "0xa117000000f279d81a1d3cc75430faa017fa5a2e",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xa117000000f279d81a1d3cc75430faa017fa5a2e"
            },
            "transferFee": 0.1
        },
        "BADGER": {
            "coingeckoId": "badger-dao",
            "decimals": 18,
            "deployedAtBlock": 11348423,
            "minOrderSize": 2,
            "quantization": 10000000000,
            "starkTokenId": "0x16c50dc7bc4d646f4348ede0cb06d82200a83439810ffc02ee671a8a2002d4c",
            "tokenAddress": "0x3472a5a71965499acd81997a54bba8d852c6e53d",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x3472a5a71965499acd81997a54bba8d852c6e53d"
            },
            "transferFee": 0.03
        },
        "BAL": {
            "coingeckoId": "balancer",
            "decimals": 18,
            "deployedAtBlock": 10299683,
            "minOrderSize": 0.7,
            "quantization": 10000000000,
            "starkTokenId": "0x8663cbfc7501a220d52f595a6d28e22c5a403613700f6ed0c3c38e7bda4281",
            "tokenAddress": "0xba100000625a3754423978a60c9317c58a424e3d",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xba100000625a3754423978a60c9317c58a424e3d"
            },
            "transferFee": 0.015
        },
        "BAT": {
            "coingeckoId": "basic-attention-token",
            "decimals": 18,
            "deployedAtBlock": 3788558,
            "minOrderSize": 20,
            "quantization": 10000000000,
            "starkTokenId": "0x3e79f4dfdbd0dea452c22801ebf43a5f01cc127cb8955be0553d7d461e1c607",
            "tokenAddress": "0x0d8775f648430679a709e98d2b0cb6250d2887ef",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0d8775f648430679a709e98d2b0cb6250d2887ef"
            },
            "transferFee": 1
        },
        "BTC": {
            "coingeckoId": "bitcoin",
            "decimals": 8,
            "deployedAtBlock": 6766284,
            "fastWithdrawalRequiredGas": 120000,
            "minOrderSize": 0.001,
            "quantization": 100,
            "starkTokenId": "0x1ff2b4f347ef6ad30e087ab8043dd7563c88c617de65cf24cd666a5fd441351",
            "tokenAddress": "0x2260fac5e5542a773aa44fbcfedf7c193bc2c599",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x2260fac5e5542a773aa44fbcfedf7c193bc2c599"
            },
            "transferFee": 2e-05
        },
        "CEL": {
            "coingeckoId": "celsius-degree-token",
            "decimals": 4,
            "deployedAtBlock": 5409020,
            "minOrderSize": 8,
            "quantization": 1,
            "starkTokenId": "0x32187f7d3db76378152d69d5ff22a5761496596ff4e91708d72d0c939d82825",
            "tokenAddress": "0xaaaebe6fe48e54f431b0c390cfaf0b017d09d42d",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xaaaebe6fe48e54f431b0c390cfaf0b017d09d42d"
            },
            "transferFee": 0.1
        },
        "COMP": {
            "coingeckoId": "compound-governance-token",
            "decimals": 18,
            "deployedAtBlock": 9601359,
            "minOrderSize": 0.07,
            "quantization": 10000000000,
            "starkTokenId": "0x5acb69e0d48a3d68e394ba2d5ceb0efc00565b80d63835b410116f293975ea",
            "tokenAddress": "0xc00e94cb662c3520282e6f5717214004a7f26888",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xc00e94cb662c3520282e6f5717214004a7f26888"
            },
            "transferFee": 0.002
        },
        "CRV": {
            "coingeckoId": "curve-dao-token",
            "decimals": 18,
            "deployedAtBlock": 10647806,
            "minOrderSize": 20,
            "quantization": 10000000000,
            "starkTokenId": "0x1ff699bcfef12cc7b9fb3c69a0c1df915e434f9cb6e3b9099515b116f12b5d",
            "tokenAddress": "0xd533a949740bb3306d119cc777fa900ba034cd52",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xd533a949740bb3306d119cc777fa900ba034cd52"
            },
            "transferFee": 0.5
        },
        "CUSDT": {
            "coingeckoId": "compound-usdt",
            "decimals": 8,
            "deployedAtBlock": 9879363,
            "maxOrderSize": 100000000,
            "minOrderSize": 300,
            "quantization": 100,
            "starkTokenId": "0x1c19dac2acd6dd66fedd77e61c65aaa022fcd928f4a0b2239bdf253f65be22c",
            "tokenAddress": "0xf650c3d88d12db855b8bf7d11be6c55a4e07dcc9",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xf650c3d88d12db855b8bf7d11be6c55a4e07dcc9"
            },
            "transferFee": 60
        },
        "DAI": {
            "coingeckoId": "dai",
            "decimals": 18,
            "deployedAtBlock": 8928158,
            "fastWithdrawalRequiredGas": 120000,
            "minOrderSize": 10,
            "quantization": 10000000000,
            "starkTokenId": "0x3db9d83c9328d408e4b27f5f8e6e97ba4dc3d0f751331c273645ce39eaaf325",
            "tokenAddress": "0x6b175474e89094c44da98b954eedeac495271d0f",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x6b175474e89094c44da98b954eedeac495271d0f",
                "MATIC_POS": "0x8f3cf7ad23cd3cadbd9735aff958023239c6a063",
                "MATIC_POS_PARENT": "0x6b175474e89094c44da98b954eedeac495271d0f"
            },
            "transferFee": 1
        },
        "DPI": {
            "coingeckoId": "defipulse-index",
            "decimals": 18,
            "deployedAtBlock": 10830516,
            "minOrderSize": 0.16,
            "quantization": 10000000000,
            "starkTokenId": "0x3cc625127856604e5aac53706d9ef78e6ca1c2fa6e9527506aa7e436bf20337",
            "tokenAddress": "0x1494ca1f11d487c2bbe4543e90080aeba4ba3c2b",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x1494ca1f11d487c2bbe4543e90080aeba4ba3c2b"
            },
            "transferFee": 0.002
        },
        "DUSK": {
            "coingeckoId": "dusk-network",
            "decimals": 18,
            "deployedAtBlock": 6867115,
            "minOrderSize": 100,
            "quantization": 10000000000,
            "starkTokenId": "0x28ac7a944aae0199887b14620ae2bbd4571e19a4553dd2419e6ca8f16d43c5f",
            "tokenAddress": "0x940a2db1b7008b6c776d4faaca729d6d4a4aa551",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x940a2db1b7008b6c776d4faaca729d6d4a4aa551"
            },
            "transferFee": 4
        },
        "DVF": {
            "coingeckoId": "deversifi",
            "decimals": 18,
            "deployedAtBlock": 12008914,
            "fastWithdrawalRequiredGas": 120000,
            "maxOrderSize": 1000000,
            "minOrderSize": 2,
            "quantization": 10000000000,
            "starkTokenId": "0x12b78656a284603f18b4f334540d7f8c7568a2da44e15532b1e8af05cf0ff64",
            "tokenAddress": "0xdddddd4301a082e62e84e43f474f044423921918",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xdddddd4301a082e62e84e43f474f044423921918"
            },
            "transferFee": 0.2
        },
        "ERP": {
            "coingeckoId": "entropyfi",
            "decimals": 18,
            "deployedAtBlock": 12008914,
            "fastWithdrawalRequiredGas": 120000,
            "maxOrderSize": 1000000,
            "minOrderSize": 50,
            "quantization": 10000000000,
            "starkTokenId": "0xf7637b1d4371911193280b9159fd059a81b8fcd4f9af0ac33099b685add019",
            "tokenAddress": "0x0a0e3bfd5a8ce610e735d4469bc1b3b130402267",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0a0e3bfd5a8ce610e735d4469bc1b3b130402267"
            },
            "transferFee": 2
        },
        "ETH": {
            "coingeckoId": "ethereum",
            "decimals": 18,
            "deployedAtBlock": 0,
            "fastWithdrawalRequiredGas": 88000,
            "minOrderSize": 0.01,
            "quantization": 10000000000,
            "starkTokenId": "0xb333e3142fe16b78628f19bb15afddaef437e72d6d7f5c6c20c6801a27fba6",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0000000000000000000000000000000000000000"
            },
            "transferFee": 0.0003
        },
        "EXRD": {
            "coingeckoId": "e-radix",
            "decimals": 18,
            "deployedAtBlock": 11138920,
            "minOrderSize": 450,
            "quantization": 10000000000,
            "starkTokenId": "0x2e58176c80cb81f92daf7f1a6826ae3f347048e759129dd78cd85a3bb158a5b",
            "tokenAddress": "0x6468e79a80c0eab0f9a2b574c8d5bc374af59414",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x6468e79a80c0eab0f9a2b574c8d5bc374af59414"
            },
            "transferFee": 10
        },
        "FUN": {
            "coingeckoId": "funfair",
            "decimals": 8,
            "deployedAtBlock": 3988945,
            "minOrderSize": 4000,
            "quantization": 100,
            "starkTokenId": "0x32d7ef7c4ed4db680494db3ebc813a2c60c00d3747e6f563799cc801b1699d5",
            "tokenAddress": "0x419d0d8bdd9af5e606ae2232ed285aff190e711b",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x419d0d8bdd9af5e606ae2232ed285aff190e711b"
            },
            "transferFee": 30
        },
        "GRT": {
            "coingeckoId": "the-graph",
            "decimals": 18,
            "deployedAtBlock": 11446769,
            "minOrderSize": 30,
            "quantization": 10000000000,
            "starkTokenId": "0x29a01c8add7b72fec5dc47cc42422b7f768d307f75fd3abff2978254b12f1f7",
            "tokenAddress": "0xc944e90c64b2c07662a292be6244bdf05cda44a7",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xc944e90c64b2c07662a292be6244bdf05cda44a7"
            },
            "transferFee": 0.5
        },
        "HEZ": {
            "coingeckoId": "hermez-network-token",
            "decimals": 18,
            "deployedAtBlock": 11056775,
            "minOrderSize": 3.5,
            "quantization": 10000000000,
            "starkTokenId": "0x2cb86b028fd5886f8adc6887f106b97da846e729e71433c72dcb8be73d67a9c",
            "tokenAddress": "0xeef9f339514298c6a857efcfc1a762af84438dee",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xeef9f339514298c6a857efcfc1a762af84438dee"
            },
            "transferFee": 0.15
        },
        "INV": {
            "coingeckoId": "inverse-finance",
            "decimals": 18,
            "deployedAtBlock": 11498340,
            "minOrderSize": 0.01,
            "quantization": 10000000000,
            "starkTokenId": "0x1a2bb1e8eb95dda77814d09e49f9f892b610d229937c3b71149fed54b33920d",
            "tokenAddress": "0x41d5d79431a913c4ae7d69a668ecdfe5ff9dfb68",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x41d5d79431a913c4ae7d69a668ecdfe5ff9dfb68"
            },
            "transferFee": 0.001
        },
        "LDO": {
            "coingeckoId": "lido-dao",
            "decimals": 18,
            "deployedAtBlock": 11473216,
            "fastWithdrawalRequiredGas": 210000,
            "maxOrderSize": 10000000,
            "minOrderSize": 25,
            "quantization": 10000000000,
            "starkTokenId": "0x25e64a8b06180f3dcb014ae5a60455cc8c676d9ad46cef9a54a5a903381b7e",
            "tokenAddress": "0x5a98fcbea516cf06857215779fd812ca3bef1b32",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x5a98fcbea516cf06857215779fd812ca3bef1b32"
            },
            "transferFee": 0.5
        },
        "LINK": {
            "coingeckoId": "chainlink",
            "decimals": 18,
            "deployedAtBlock": 4281611,
            "minOrderSize": 1,
            "quantization": 10000000000,
            "starkTokenId": "0x155d72fdf10a9b48e53a4dafc07777588ab028775aaccfac7fbebfbe1d9f7b0",
            "tokenAddress": "0x514910771af9ca656af840dff83e8264ecf986ca",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x514910771af9ca656af840dff83e8264ecf986ca"
            },
            "transferFee": 0.03
        },
        "LRC": {
            "coingeckoId": "loopring",
            "decimals": 18,
            "deployedAtBlock": 7544036,
            "minOrderSize": 85,
            "quantization": 10000000000,
            "starkTokenId": "0x109357cc6366baceb779c26ce6a670c70de91e0f889f23eb20e49e053919423",
            "tokenAddress": "0xbbbbca6a901c926f240b89eacb641d8aec7aeafd",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xbbbbca6a901c926f240b89eacb641d8aec7aeafd"
            },
            "transferFee": 1
        },
        "MATIC": {
            "coingeckoId": "matic-network",
            "decimals": 18,
            "deployedAtBlock": 12008914,
            "minOrderSize": 10,
            "quantization": 10000000000,
            "starkTokenId": "0x29ed085d11df04b59ba5830088d9ecd19c51834375a988257a1e3ff6ef82020",
            "tokenAddress": "0x7d1afa7b718fb893db30a3abc0cfc608aacfebb0",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x7d1afa7b718fb893db30a3abc0cfc608aacfebb0"
            },
            "transferFee": 0.5
        },
        "MKR": {
            "coingeckoId": "maker",
            "decimals": 18,
            "deployedAtBlock": 4620855,
            "minOrderSize": 0.01,
            "quantization": 10000000000,
            "starkTokenId": "0x1a4af39d27ce2e3445ed084809e5bc36d03918df04b7e2b6ee3c769a9892600",
            "tokenAddress": "0x9f8f72aa9304c8b593d555f12ef6589cc3a579a2",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x9f8f72aa9304c8b593d555f12ef6589cc3a579a2"
            },
            "transferFee": 0.0002
        },
        "MLN": {
            "coingeckoId": "melon",
            "decimals": 18,
            "deployedAtBlock": 7130380,
            "minOrderSize": 0.2,
            "quantization": 10000000000,
            "starkTokenId": "0x17e258e6c7dc57c8b9507c1cce0a7a18565ef0d1af1242945ef4e44b7dda1d4",
            "tokenAddress": "0xec67005c4e498ec7f55e092bd1d35cbc47c91892",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xec67005c4e498ec7f55e092bd1d35cbc47c91892"
            },
            "transferFee": 0.02
        },
        "NEC": {
            "coingeckoId": "nectar-token",
            "decimals": 18,
            "deployedAtBlock": 5072026,
            "minOrderSize": 50,
            "quantization": 10000000000,
            "starkTokenId": "0x2c27851c648a31b4f5e2253a5bba3e61382a83a4daeb2a905f74757297f391d",
            "tokenAddress": "0xcc80c051057b774cd75067dc48f8987c4eb97a5e",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xcc80c051057b774cd75067dc48f8987c4eb97a5e"
            },
            "transferFee": 5
        },
        "NU": {
            "coingeckoId": "nucypher",
            "decimals": 18,
            "deployedAtBlock": 10763456,
            "minOrderSize": 121,
            "quantization": 10000000000,
            "starkTokenId": "0x319333841362da037e36a9bf3361f9f232a3dea6c91c12aeb25148bd9f34b76",
            "tokenAddress": "0x4fe83213d56308330ec302a8bd641f1d0113a4cc",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x4fe83213d56308330ec302a8bd641f1d0113a4cc"
            },
            "transferFee": 2
        },
        "OMG": {
            "coingeckoId": "omisego",
            "decimals": 18,
            "deployedAtBlock": 3978297,
            "minOrderSize": 10,
            "quantization": 10000000000,
            "starkTokenId": "0x520528c3d1ad53a721231ec1f92227d37a14f3fd852fabdd261eb96227d031",
            "tokenAddress": "0xd26114cd6EE289AccF82350c8d8487fedB8A0C07",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xd26114cd6EE289AccF82350c8d8487fedB8A0C07"
            },
            "transferFee": 0.2
        },
        "PNK": {
            "coingeckoId": "kleros",
            "decimals": 18,
            "deployedAtBlock": 5257012,
            "minOrderSize": 250,
            "quantization": 10000000000,
            "starkTokenId": "0x2c77fdc97759f654a74b6ba9845219df635f53ffa877bdfc69f4dbf7028885a",
            "tokenAddress": "0x93ed3fbe21207ec2e8f2d3c3de6e058cb73bc04d",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x93ed3fbe21207ec2e8f2d3c3de6e058cb73bc04d"
            },
            "transferFee": 5
        },
        "REN": {
            "coingeckoId": "republic-protocol",
            "decimals": 18,
            "deployedAtBlock": 4827494,
            "minOrderSize": 60,
            "quantization": 10000000000,
            "starkTokenId": "0x2541a6e2385351071782cd14739f74f351b83cfe173a2bcd6134d53eb130617",
            "tokenAddress": "0x408e41876cccdc0f92210600ef50372656052a38",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x408e41876cccdc0f92210600ef50372656052a38"
            },
            "transferFee": 1
        },
        "ROOK": {
            "coingeckoId": "rook",
            "decimals": 18,
            "deployedAtBlock": 11169699,
            "minOrderSize": 0.14,
            "quantization": 10000000000,
            "starkTokenId": "0x161247c2a777dd41f0f7f75071c999c25825208d1fda112dbcb20554752713d",
            "tokenAddress": "0xfa5047c9c78b8877af97bdcb85db743fd7313d4a",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xfa5047c9c78b8877af97bdcb85db743fd7313d4a"
            },
            "transferFee": 0.0025
        },
        "RUNE": {
            "coingeckoId": "thorchain",
            "decimals": 18,
            "deployedAtBlock": 11644425,
            "minOrderSize": 3.5,
            "quantization": 10000000000,
            "starkTokenId": "0x3e46c2e13cc9f28339bbb2ba202c993ec19e535b2aa8ee3fae051b0b648fc70",
            "tokenAddress": "0x3155ba85d5f96b2d030a4966af206230e46849cb",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x3155ba85d5f96b2d030a4966af206230e46849cb"
            },
            "transferFee": 0.1
        },
        "SHIB": {
            "coingeckoId": "shiba-inu",
            "decimals": 18,
            "deployedAtBlock": 12008914,
            "minOrderSize": 100000,
            "quantization": 10000000000,
            "starkTokenId": "0x81aa49c199a78e0a085fc5552cc9fa460b111a730d2e4cd37ac8dd58ba117",
            "tokenAddress": "0x95ad61b0a150d79219dcf64e1e6cc01f0b64c4ce",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x95ad61b0a150d79219dcf64e1e6cc01f0b64c4ce"
            },
            "transferFee": 10000
        },
        "SNX": {
            "coingeckoId": "havven",
            "decimals": 18,
            "deployedAtBlock": 8314597,
            "minOrderSize": 3.5,
            "quantization": 10000000000,
            "starkTokenId": "0x1e2ae6df91bdab7e2fc34aa064d36314d4e2a6fb5b0399c4a12c552f38a22ba",
            "tokenAddress": "0xc011a73ee8576fb46f5e1c5751ca3b9fe0af2a6f",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xc011a73ee8576fb46f5e1c5751ca3b9fe0af2a6f"
            },
            "transferFee": 0.04
        },
        "SUSHI": {
            "coingeckoId": "sushi",
            "decimals": 18,
            "deployedAtBlock": 10736094,
            "minOrderSize": 2,
            "quantization": 10000000000,
            "starkTokenId": "0x1aea146c03bc7bd2102a65ae9bccb23246e319b17dcf88fdd0d1029a417b7d",
            "tokenAddress": "0x6b3595068778dd592e39a122f4f5a5cf09c90fe2",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x6b3595068778dd592e39a122f4f5a5cf09c90fe2"
            },
            "transferFee": 0.05
        },
        "TORN": {
            "coingeckoId": "tornado-cash",
            "decimals": 18,
            "deployedAtBlock": 11474599,
            "minOrderSize": 0.3,
            "quantization": 10000000000,
            "starkTokenId": "0x3aad1b58d18778c117786431aea79acb4f4a9581992b2adda19af7f892f84da",
            "tokenAddress": "0x77777feddddffc19ff86db637967013e6c6a116c",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x77777feddddffc19ff86db637967013e6c6a116c"
            },
            "transferFee": 0.01
        },
        "UNI": {
            "coingeckoId": "uniswap",
            "decimals": 18,
            "deployedAtBlock": 10861674,
            "minOrderSize": 2,
            "quantization": 10000000000,
            "starkTokenId": "0x52f7a6e9735bee915ecc2b45f716cc7469ec70fdd75e946c87dfce75ef33b3",
            "tokenAddress": "0x1f9840a85d5af5bf1d1762f925bdaddc4201f984",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x1f9840a85d5af5bf1d1762f925bdaddc4201f984"
            },
            "transferFee": 0.03
        },
        "USDC": {
            "coingeckoId": "usd-coin",
            "decimals": 6,
            "deployedAtBlock": 6082465,
            "fastWithdrawalRequiredGas": 120000,
            "minOrderSize": 10,
            "quantization": 1,
            "starkTokenId": "0x2893294412a4c8f915f75892b395ebbf6859ec246ec365c3b1f56f47c3a0a5d",
            "tokenAddress": "0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48",
                "MATIC_POS": "0x2791bca1f2de4661ed88a30c99a7a9449aa84174",
                "MATIC_POS_PARENT": "0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48"
            },
            "transferFee": 1
        },
        "USDT": {
            "bitfinexWithdrawalAddress": "0x50f28352380f297b29b3318c1222537b2e58a086",
            "coingeckoId": "tether",
            "decimals": 6,
            "deployedAtBlock": 4634748,
            "fastWithdrawalRequiredGas": 120000,
            "minOrderSize": 10,
            "quantization": 1,
            "settleSpread": 0,
            "starkTokenId": "0x2ce625e94458d39dd0bf3b45a843544dd4a14b8169045a3a3d15aa564b936c5",
            "tokenAddress": "0xdac17f958d2ee523a2206206994597c13d831ec7",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xdac17f958d2ee523a2206206994597c13d831ec7",
                "MATIC_POS": "0xc2132d05d31c914a87c6611c10748aeb04b58e8f",
                "MATIC_POS_PARENT": "0xdac17f958d2ee523a2206206994597c13d831ec7"
            },
            "transferFee": 1
        },
        "WSTETH": {
            "coingeckoId": "staked-ether",
            "decimals": 18,
            "deployedAtBlock": 11888477,
            "minOrderSize": 0.03,
            "quantization": 10000000000,
            "starkTokenId": "0x16d3117c099642acfca604786a73984987728d7fc02690f598c1118b588fb38",
            "tokenAddress": "0x7f39c581f595b53c5cb19bd0b3f8da6c935e2ca0",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x7f39c581f595b53c5cb19bd0b3f8da6c935e2ca0"
            },
            "transferFee": 0.0003
        },
        "YFI": {
            "coingeckoId": "yearn-finance",
            "decimals": 18,
            "deployedAtBlock": 10475744,
            "minOrderSize": 0.0007,
            "quantization": 10000000000,
            "starkTokenId": "0x200068154b056d930907d57ee87a7a3a69a8eb2616f4582a3c2d1758c69b8e3",
            "tokenAddress": "0x0bc529c00C6401aEF6D220BE8C6Ea1667F6Ad93e",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0bc529c00C6401aEF6D220BE8C6Ea1667F6Ad93e"
            },
            "transferFee": 3e-05
        },
        "ZRX": {
            "coingeckoId": "0x",
            "decimals": 18,
            "deployedAtBlock": 4145415,
            "minOrderSize": 20,
            "quantization": 10000000000,
            "starkTokenId": "0x26ce9f287ea325c031bafdc647f27b331e864a0661aedb5ebdfb1b671289667",
            "tokenAddress": "0xe41d2489571d322189246dafa5ebde1f4699f498",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xe41d2489571d322189246dafa5ebde1f4699f498"
            },
            "transferFee": 0.5
        },
        "wXNM": {
            "coingeckoId": "wrapped-nxm",
            "decimals": 18,
            "deployedAtBlock": 10383026,
            "minOrderSize": 0.6,
            "quantization": 10000000000,
            "starkTokenId": "0x1a2b7abf32289a4d367838371b585a15c998a0939511b8b5ffb89afae92de68",
            "tokenAddress": "0x0d438f3b5175bebc262bf23753c1e53d03432bde",
            "tokenAddressPerChain": {
                "ETHEREUM": "0x0d438f3b5175bebc262bf23753c1e53d03432bde"
            },
            "transferFee": 0.01
        },
        "xDVF": {
            "coingeckoId": "deversifi",
            "decimals": 18,
            "deployedAtBlock": 12554375,
            "maxOrderSize": 1000000,
            "minOrderSize": 2,
            "quantization": 10000000000,
            "starkTokenId": "0x2f1ac180be47ec22c2315cc442d53d92f3be8e1d0249263e6598cf4ecddab78",
            "tokenAddress": "0xdddd0e38d30dd29c683033fa0132f868597763ab",
            "tokenAddressPerChain": {
                "ETHEREUM": "0xdddd0e38d30dd29c683033fa0132f868597763ab"
            },
            "transferFee": 0.2
        }
    }
}
```