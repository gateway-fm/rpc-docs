---
description: Returns traces matching given filter
---

# trace\_filter

#### **Parameters**

* `Object` - The filter object
  * `fromBlock`: `Quantity` or `Tag` - (optional) From this block.
  * `toBlock`: `Quantity` or `Tag` - (optional) To this block.
  * `fromAddress`: `Array` - (optional) Sent from these addresses.
  * `toAddress`: `Address` - (optional) Sent to these addresses.
  * `after`: `Quantity` - (optional) The offset trace number
  * `count`: `Quantity` - (optional) Integer number of traces to display in a batch.

#### **Returns**

`Array` - Block traces.

``

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"method":"trace_filter","params":[{"fromBlock":"0x2ed0c4","toBlock":"0x2ed128","toAddress":["0x8bbB73BCB5d553B5A556358d27625323Fd781D37"],"after":1000,"count":100}],"id":1,"jsonrpc":"2.0"}'
```

Result

```javascript
{
  "id": 1,
  "jsonrpc": "2.0",
  "result": [
    {
      "action": {
        "callType": "call",
        "from": "0x32be343b94f860124dc4fee278fdcbd38c102d88",
        "gas": "0x4c40d",
        "input": "0x",
        "to": "0x8bbb73bcb5d553b5a556358d27625323fd781d37",
        "value": "0x3f0650ec47fd240000"
      },
      "blockHash": "0x86df301bcdd8248d982dbf039f09faf792684e1aeee99d5b58b77d620008b80f",
      "blockNumber": 3068183,
      "result": {
        "gasUsed": "0x0",
        "output": "0x"
      },
      "subtraces": 0,
      "traceAddress": [],
      "transactionHash": "0x3321a7708b1083130bd78da0d62ead9f6683033231617c9d268e2c7e3fa6c104",
      "transactionPosition": 3,
      "type": "call"
    },
    ...
  ]
}
```
