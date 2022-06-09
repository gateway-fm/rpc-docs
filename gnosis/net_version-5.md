---
description: >-
  Traces a call to eth_sendRawTransaction without making the call, returning the
  traces
---

# trace\_rawTransaction

#### **Parameters**

* `Data` - Raw transaction data
*   `Array` - Type of trace, one or more of: `"vmTrace"`, `"trace"`, `"stateDiff"`.

    ``

#### **Returns**

`Object` - Block traces.

``

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"method":"trace_rawTransaction","params":["0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675",["trace"]],"id":1,"jsonrpc":"2.0"}'
```

Result

```javascript

  "id": 1,
  "jsonrpc": "2.0",
  "result": {
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
    "vmTrace": null
  }
}
```
