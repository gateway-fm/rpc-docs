---
description: This method is used to get the history of fills (executed trades) for the authenticated user
---
# Fills history

### **Parameters**
none

### **Returns**
`pagination` - object

    `totalItems` - number; Total number of items matching the query
    
    `limit` - number; Limit applied on returned items
    
    `skip` - number; Skip applied on returned items

`items` - object

`_id` - string; Unique identifier representing this transfer

    `token` - string; Token transfered
    
    `amount` - number; Amount transfered (effective amount received by the recipient)
    
    `feeAmount` - number; Transfer fee amount (in transfer token units)
    
    `source` - string; Source Ethereum address
    
    `recipient` - string; Recipient Ethereum address
    
    `date` - string; Date and time of the transfer

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/fills \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json"
```


Result

```javascript
{
  "items": [
    {
      "_id": "KXUPSDQ1arf",
      "token": "ETH",
      "amount": 0.3,
      "recipient": "0x271f6a30fcf762325d3213ce19ed55e7e6a8cac1",
      "source": "0x271f6a30fcf762325d3213ce19ed55e7e6a8cac1",
      "date": "2021-03-03T10:46:28.630Z",
      "feeAmount": 0
    }
  ],
  "pagination": {
    "totalItems": 5,
    "skip": 0,
    "limit": 20
  }
}
```