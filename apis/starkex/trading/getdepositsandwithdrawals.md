---
description: An authenticated endpoint used to retrieve history of deposits and withdrawals
---
# Get deposits and withdrawal history

### **Parameters**
`skip` - number; Include/exclude details

`sortDirection` - string; Sorting option

### **Returns**

`items` - array; Transaction details

`pagination` - object

`totalItems` - number; Total number of items matching the query

`limit` - number; Limit applied on returned items

`skip` - number; Skip applied on returned items

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/{prod|stg}/trading/depositsAndWithdrawals?skip=0&sortDirection=DESC \
-X GET \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
```


Result

```javascript
{
    "items": [
        {
            "_id": "2RNJXrzxpsR",
            "type": "Deposit",
            "token": "ETH",
            "amount": 0.06,
            "transactionHash": "0xd1a8c36d7958a1d552709555641b378899a1119bb8a8a2a5d9669e545cb63427",
            "date": "2021-11-25T12:42:05.000Z",
            "sourceOrRecipient": "0x6619328e32ea172d0a9bcbf27550e1a43663ec44"
        }
    ],
    "pagination": {
        "totalItems": 1,
        "skip": 0,
        "limit": 20
    }
}