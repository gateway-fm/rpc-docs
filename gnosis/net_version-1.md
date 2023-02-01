---
description: Returns traces created at given block.
---

# trace_block

#### **Parameters**

`Quantity` or `Tag` - Integer of a block number, or the string `'earliest'`, `'latest'` or `'pending'`one

#### **Returns**

`Array` - Block traces.

``

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v4/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"method":"trace_block","params":["0xccb93d"],"id":1,"jsonrpc":"2.0"}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "result": [
        {
            "action": {
                "callType": "call",
                "from": "0x9526818a8f5d997652c213a28cc532cf6b709aa4",
                "gas": "0x71711",
                "input": "0x3d18b912",
                "to": "0x74f267b4dfe414f493d97eb6012ef1b61306247d",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x496c7",
                "output": "0x"
            },
            "subtraces": 1,
            "traceAddress": [],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x74f267b4dfe414f493d97eb6012ef1b61306247d",
                "gas": "0x601ab",
                "input": "0xa9059cbb0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x3931a",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 1,
            "traceAddress": [
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "gas": "0x5b1c0",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x23daa",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 2,
            "traceAddress": [
                0,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x58c71",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0fd8de493821904a0eae23e3a30ab559947038f8683de280e97f786d5b2ed59f7c",
                "to": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x12be",
                "output": "0x0000000000000000000000006cf875264151f011fb9173889b901fa544dc4bc7"
            },
            "subtraces": 1,
            "traceAddress": [
                0,
                0,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "gas": "0x55c51",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0fd8de493821904a0eae23e3a30ab559947038f8683de280e97f786d5b2ed59f7c",
                "to": "0x336ebb4def4da4fad6936874b8c952e800024653",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x6b9",
                "output": "0x0000000000000000000000006cf875264151f011fb9173889b901fa544dc4bc7"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                0,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x56481",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x6cf875264151f011fb9173889b901fa544dc4bc7",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x21486",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 4,
            "traceAddress": [
                0,
                0,
                1
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x53bc0",
                "input": "0x70a082310000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa4",
                "to": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x2021",
                "output": "0x000000000000000000000000000000000000000000000000000018a346c25142"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x510ef",
                "input": "0x70a0823100000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d",
                "to": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x2021",
                "output": "0x0000000000000000000000000000000000000000000000003179a49be7a47f47"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                1
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x4d47f",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x00f9092e5806628d7a44e496c503cec608e64f1f",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0xc62b",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 2,
            "traceAddress": [
                0,
                0,
                1,
                2
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x00f9092e5806628d7a44e496c503cec608e64f1f",
                "gas": "0x4b2a5",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0f82d8d87cd48f4b245d5c8c1c98c5d527dc7b7e166f62471569fb8b1061900644",
                "to": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x12be",
                "output": "0x000000000000000000000000a2c57a91d9432a685b1df6ecbb61d6063d35808a"
            },
            "subtraces": 1,
            "traceAddress": [
                0,
                0,
                1,
                2,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "gas": "0x48285",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0f82d8d87cd48f4b245d5c8c1c98c5d527dc7b7e166f62471569fb8b1061900644",
                "to": "0x336ebb4def4da4fad6936874b8c952e800024653",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x6b9",
                "output": "0x000000000000000000000000a2c57a91d9432a685b1df6ecbb61d6063d35808a"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                2,
                0,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0x00f9092e5806628d7a44e496c503cec608e64f1f",
                "gas": "0x48740",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0xa2c57a91d9432a685b1df6ecbb61d6063d35808a",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x9d07",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 1,
            "traceAddress": [
                0,
                0,
                1,
                2,
                1
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x00f9092e5806628d7a44e496c503cec608e64f1f",
                "gas": "0x40372",
                "input": "0x981b24d00000000000000000000000000000000000000000000000000000000000000000",
                "to": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x1002",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000000"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                2,
                1,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x2118c3343f6d6d7a2b2ff68c82581cc188166d54",
                "gas": "0x3f90c",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x7f67f5de7b815c5709be70f5eea627de43bb1b0c",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0xb517",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 2,
            "traceAddress": [
                0,
                0,
                1,
                3
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x7f67f5de7b815c5709be70f5eea627de43bb1b0c",
                "gas": "0x3da9f",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0fabb88ccde8e73f80a3f4a14ef4f6bbfcc19f172a073a5d4cace3af06a8f2a182",
                "to": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x12be",
                "output": "0x0000000000000000000000006a992a38c8780b040657a6f83049e838b9575abd"
            },
            "subtraces": 1,
            "traceAddress": [
                0,
                0,
                1,
                3,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0xe9869a0bbc8fb8c61b7d81c33fa2ba84871b3b0e",
                "gas": "0x3aa7f",
                "input": "0xbe00bbd8f1f3eb40f5bc1ad1344716ced8b8a0431d840b5783aea1fd01786bc26f35ac0fabb88ccde8e73f80a3f4a14ef4f6bbfcc19f172a073a5d4cace3af06a8f2a182",
                "to": "0x336ebb4def4da4fad6936874b8c952e800024653",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x6b9",
                "output": "0x0000000000000000000000006a992a38c8780b040657a6f83049e838b9575abd"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                3,
                0,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "delegatecall",
                "from": "0x7f67f5de7b815c5709be70f5eea627de43bb1b0c",
                "gas": "0x3abcd",
                "input": "0x4a39314900000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d0000000000000000000000009526818a8f5d997652c213a28cc532cf6b709aa400000000000000000000000000000000000000000000000000021417a8478dcd",
                "to": "0x6a992a38c8780b040657a6f83049e838b9575abd",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x8bf3",
                "output": "0x0000000000000000000000000000000000000000000000000000000000000001"
            },
            "subtraces": 1,
            "traceAddress": [
                0,
                0,
                1,
                3,
                1
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        },
        {
            "action": {
                "callType": "call",
                "from": "0x7f67f5de7b815c5709be70f5eea627de43bb1b0c",
                "gas": "0x33e5b",
                "input": "0x70a0823100000000000000000000000074f267b4dfe414f493d97eb6012ef1b61306247d",
                "to": "0x71850b7e9ee3f13ab46d67167341e4bdc905eef9",
                "value": "0x0"
            },
            "blockHash": "0x122d4887521e526c41847cd1cacbb686764322c3e40d6c118b91fca99e6f0b36",
            "blockNumber": 13416765,
            "result": {
                "gasUsed": "0x2021",
                "output": "0x0000000000000000000000000000000000000000000000003179a49be7a47f47"
            },
            "subtraces": 0,
            "traceAddress": [
                0,
                0,
                1,
                3,
                1,
                0
            ],
            "transactionHash": "0xd3467cd285b23cd7312e43fd91d58991094a62d661fbbe1cc816c276b37e96a2",
            "transactionPosition": 0,
            "type": "call"
        }
    ],
    "id": 1
}
```
