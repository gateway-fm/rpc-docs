---
description: Returns the current network id.
---

# net_version

#### **Parameters**

none

#### **Returns**

`String` - The current network id.

`"1"`: Ethereum Mainnet
`"2"`: Morden Testnet (deprecated)
`"3"`: Ropsten Testnet
`"4"`: Rinkeby Testnet
`"42"`: Kovan Testnet

### **Example**
Request

```bash
curl https://rpc.gateway.fm/v1/ethereum/mainnet \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "Content-Type: application/json" \
-d '{ "id": 89, "jsonrpc": "2.0", "method": "net_version", "params": []}'
```
Result

```javascript
{
    "jsonrpc":"2.0",
    "id":89,
    "result":"1"
}
```
