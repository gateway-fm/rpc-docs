---
description: >-
  Replays all transactions in a block returning the requested traces for each
  transaction.
---

# trace\_replayBlockTransaction

#### **Parameters**

1. `Quantity` or `Tag` - Integer of a block number, or the string `'earliest'`, `'latest'` or `'pending'`.
2. `Array` - Type of trace, one or more of: `"vmTrace"`, `"trace"`, `"stateDiff"`

#### **Returns**

`Array` - Block transactions traces.

``

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"method":"trace_replayBlockTransactions","params":["0x2ed119",["trace"]],"id":1,"jsonrpc":"2.0"}'
```

Result

```javascript
{
  "id": 1,
  "jsonrpc": "2.0",
  "result": [
    {
      "output": "0x",
      "stateDiff": null,
      "trace": [{
        "action": { ... },
        "result": {
          "gasUsed": "0x0",
          "output": "0x"
        },
        "subtraces": 0,
        "traceAddress": [],
        "type": "call"
      }],
      "transactionHash": "0x...",
      "vmTrace": null
    },
    { ... }
  ]
}
```
