---
description: Executes the given call and returns a number of possible traces for it.
---

# trace_call

#### **Parameters**

`object` - The transaction object, which contains of

`from` - (optional) String of the address the transaction is sent from.

`to` - String of the address the transaction is directed to.

`gas` - (optional) Integer of the gas provided for the transaction execution.

`gasprice` - (optional) Integer of the gasPrice used for each paid gas encoded as a hexadecimal.

`value` - (optional) Integer of the value sent with this transaction encoded as a hexadecimal.

`data` - (optional) String of the hash of the method signature and encoded parameters

`array` - Type of trace, one or more of `vmTrace` ,`trace` ,`statediff`&#x20;

`quantity` or `tag` - Integer block number, or the string 'latest', 'earliest' or 'pending'

#### **Returns**

`Array` - Block traces.

``

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v4/gnosis/non-archival/mainnet \
-X POST \
-H "Content-Type: application/json" \
-d '{"method":"trace_call","params":[{ ... },["trace"]],"id":1,"jsonrpc":"2.0"}'
```

Result

```javascript
{
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
