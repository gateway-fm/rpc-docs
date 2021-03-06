---
description: This endpoint allows to cancel a specific order.
---
# Cancel Order

### **Parameters**

`orderId` - string
The order ID.

`cid` - string
An optional user-defined identifier for this order

### **Returns**
`orderId` - string
The order ID.

`canceled` - boolean
only if order is already canceled

#### **Example**

Request

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/w/cancelOrder \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: <EcRecover_value>" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \  
-d '{"orderId": "d7c8b9"}'
```


Result

```javascript
{
  "orderId": "d7c8b9"
}
```
