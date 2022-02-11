---
description: Returns a collection of historical gas information
---

# eth\_feeHistory

**Parameters**

* `BLOCKCOUNT` - Number of blocks in the requested range. Between 1 and 1024 blocks can be requested in a single query. Less than requested may be returned if not all blocks are available.
* `NEWESTBLOCK` - Highest number block of the requested range.
* `REWARDPERCENTILES` - \(optional\) A monotonically increasing list of percentile values to sample from each block's effective priority fees per gas in ascending order, weighted by gas used.

**Returns**

`Object`

* `OLDESTBLOCK` - Lowest number block of the returned range.
* `BASEFEEPERGAS` - An array of block base fees per gas. This includes the next block after the newest of the returned range, because this value can be derived from the newest block. Zeroes are returned for pre-EIP-1559 blocks.
* `GASUSEDRATIO` - An array of block gas used ratios. These are calculated as the ratio of gasUsed and gasLimit.
* `REWARD` - \(Optional\) An array of effective priority fee per gas data points from a single block. All zeroes are returned if the block is empty. 

**Example**

Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/rinkeby \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_feeHistory","params":[4, "latest", [3, 10]],"id":1}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": {
        "baseFeePerGas": [
            "0xfc64c81be",
            "0x102b65e903",
            "0xea6002ba3",
            "0xdb1712831",
            "0xe8ee3d266"
        ],
        "gasUsedRatio": [
            0.6001403962364085,
            0.1237159,
            0.23913748224858425,
            0.7526904013787193
        ],
        "oldestBlock": "0xd873a3",
        "reward": [
            [
                "0xed12642",
                "0x59682f00"
            ],
            [
                "0x59682f00",
                "0x59682f00"
            ],
            [
                "0x3b9aca00",
                "0x3b9aca00"
            ],
            [
                "0x3b9aca00",
                "0x46d62fcf"
            ]
        ]
    }
}
```

