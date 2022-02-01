---
description: Returns information about a block by block number.
---

# eth\_getBlockByNumber

### Parameters

Parameters

QUANTITY|TAG - integer of a block number, or the string "earliest", "latest" or "pending", as in the default block parameter.

Boolean - If true it returns the full transaction objects, if false only the hashes of the transactions.

```javascript
params: [
'0x26C4FE', // 436
true
]
```

### Returns

See [`eth_getBlockByHash`](./#eth_getblockbyhash)

### Example
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 89, "jsonrpc": "2.0", "method": "eth_getBlockByNumber", "params": [     "0x26C4FE",     false ]}'
```

Result

```javascript
{
    "jsonrpc":"2.0",
    "id":89,
    "result":
        {
            "difficulty":"0x4a492bd9194b",
            "extraData":"0x65746865726d696e65202d20455531",
            "gasLimit":"0x1e78d7",
            "gasUsed":"0x42290",
            "hash":"0x7b413911f45f4691fe9469e6266c4a76244d2d0b7b5707f727a0e09ed05be972",
            "logsBloom":"0x00000000000000000000000000000002000000000000000000100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000000000000000000",
            "miner":"0xea674fdde714fd979de3edf0f56aa9716b898ec8",
            "mixHash":"0x9f0f0af54f06b51b3d070bc840f6a8242a13f50ac6df9e163cf292471d3d2cf3",
            "nonce":"0x32f35a803a58bb4e",
            "number":"0x26c4fe",
            "parentHash":"0x4b431311f67ba93dfa564b3a17db67b42b38e6d877547a2a9cfbfd3e72a1ba75",
            "receiptsRoot":"0x4f21018c3ba2e3d8fc3946193aad37955a3b2b75f4d706844342e93f3d325e98",
            "sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
            "size":"0x793",
            "stateRoot":"0xcfd1d0e05809eeccf885eb8f5e62ba43abeedb18a3a9eb3aca993a7110b736dd",
            "timestamp":"0x58172aa9",
            "totalDifficulty":"0x49344accb920392f2",
            "transactions":["0x75dbe583e035a12d5a937a57d7c8950e5a70328f1266f5ece8509d2ac32d6e22","0x91a70d8fe8c3bb94f2e5ad9294ebe0acbc28aabf0b40e567a11e471f9e4fe949","0x676abab66485a08529c6d897619e2f67fca1f808df416cb44a5b542863134fe5","0xdf23c69d89b156da14a5e64d015405bbf5e63463da25cf25739e1d32661b5209","0x9a2360c8b455ae4bac979a31031e0414b921acc40bce944b8d5ab23d87be5021","0xae91c15ee43a740b505cd6bf520bc2170a69fd63b9fb0b9789b75cfacdb6110a","0xd672558566299fe76a105a16e001711ad5d4512c06cfc7754a26710a01e90fa7","0xe4b4e2ac61cec2a764cb8fbf69d242e5305b3cbb041e28714153411fdb53b4bd","0x9ff1757f092b0945948c6c91143a9aaafd2937434c6835a8b11f1cc6e8536d03","0x221a390815ff41c4218f536b679bbbeddfba52f680877ec704b7418469f88c32","0x1fe5880bad631279c7a00a3e00dc6b4557ed28c948c1b1a8198b2b18be0b8b55","0x0b984579f895745f63ebc633cc229f503994998bf7858c82ab6674627d8a56a2"],
            "transactionsRoot":"0x982d7e34bf1ad458dc019e5fae3088439e3fcb83bd89289dee403e49d9f7e62c",
            "uncles":[]
          }
}
```

