---
description: An authenticated endpoint used to withdraw token  
---
# Fast withdrawal

### **Parameters**


### **Returns**


#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/w/fastWithdrawal \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{
   "recipientEthAddress":"0x55ba4cb41d0c8f62ab4bb207d0bf9fa42f9fe70d",
   "transactionFee":"67726954",
   "tx":{
      "amount":"178726954",
      "fact":"6d66ab64445d5f284729a66497603d6caed81913c0e5bba5a6d8dfb9367060dd",
      "factRegistryAddress":"0x53AF4f40b647D5E939B1e81356883A845cc9E7b6",
      "nonce":1007100875,
      "receiverPublicKey":"0x003cafee3970eb7338cdd9118343f328087474ddb67aa1f572de044333a17d59",
      "receiverVaultId":1220796649,
      "senderVaultId":1251139047,
      "token":"0x4507594b0258664463ad7bd1d1e9b1ff67821113abd1b9c7e082bb304da322",
      "type":"ConditionalTransferRequest",
      "senderPublicKey":"0x02505c68d1a563972b3b1c6ebd9bc3556cab07be90ebd24b8fe985b88c28129c",
      "expirationTimestamp":889072,
      "signature":{
         "r":"0x6c675ef889cd755576331b16f706e4adec70ad2e0da623def1dd0b931682a84",
         "s":"0x1a96a7586664553f40ce1c9a7f61ee97b30d5c016e55335fe2acfd85f54dce6"
      }
   },
   "starkPublicKey":{
      "x":"02505c68d1a563972b3b1c6ebd9bc3556cab07be90ebd24b8fe985b88c28129c",
      "y":"220f051a7cbd4d28eff5bac09f0be7474123cd07b063543511f4d94595f9007"
   }
}'
```


Result

```javascript
{
    "readyToWithdrawOnChain": false,
    "token": "USDT",
    "amount": "178726954",
    "fastWithdrawalData": {
        "transactionFee": "67726954",
        "recipientEthAddress": "0x55ba4cb41d0c8f62ab4bb207d0bf9fa42f9fe70d",
        "onChain": {
            "amount": "111000000"
        }
    },
    "_id": "GtNehGRD6jz",
    "createdAt": "2022-02-21T16:33:27.482Z"
}