---
description: Returns the hash of the current block, the seedHash, and the boundary condition to be met (“target”).
---

# eth\_getWork

### Parameters

none

### Returns

`Array` - Array with the following properties:
    `DATA`, 32 Bytes - current block header pow-hash
    `DATA`, 32 Bytes - the seed hash used for the DAG.
    `DATA`, 32 Bytes - the boundary condition (“target”), 2^256 / difficulty.

### [Example]
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_getWork","params":[],"id":1}'
```

Result

```javascript
{
  "id":1,
  "jsonrpc":"2.0",
  "result": [
      "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef",
      "0x5EED00000000000000000000000000005EED0000000000000000000000000000",
      "0xd1ff1c01710000000000000000000000d1ff1c01710000000000000000000000"
    ]
}
```

