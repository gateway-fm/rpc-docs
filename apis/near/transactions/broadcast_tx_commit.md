---
description: Sends a transaction and waits until transaction is fully complete. 
---

# Send transaction (await)

### **Parameters**
* `method:` broadcast_tx_commit
* `params:` [SignedTransaction encoded in base64]

### **Returns**
Sends a transaction and waits until transaction is fully complete. (Has a 10 second timeout)

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "11",
  "method": "broadcast_tx_commit",
  "params": [
    "DgAAAHNlbmRlci50ZXN0bmV0AOrmAai64SZOv9e/naX4W15pJx0GAap35wTT1T/DwcbbDQAAAAAAAAAQAAAAcmVjZWl2ZXIudGVzdG5ldIODI4YfV/QS++blXpQYT+bOsRblTRW4f547y/LkvMQ9AQAAAAMAAACh7czOG8LTAAAAAAAAAAXcaTJzu9GviPT7AD4mNJGY79jxTrjFLoyPBiLGHgBi8JK1AnhK8QknJ1ourxlvOYJA2xEZE8UR24THmSJcLQw="
  ]
}'
```

Result

```javascript
{
  "jsonrpc": "2.0",
  "result": {
    "status": {
      "SuccessValue": ""
    },
    "transaction": {
      "signer_id": "sender.testnet",
      "public_key": "ed25519:Gowpa4kXNyTMRKgt5W7147pmcc2PxiFic8UHW9rsNvJ6",
      "nonce": 13,
      "receiver_id": "receiver.testnet",
      "actions": [
        {
          "Transfer": {
            "deposit": "1000000000000000000000000"
          }
        }
      ],
      "signature": "ed25519:7oCBMfSHrZkT7tzPDBxxCd3tWFhTES38eks3MCZMpYPJRfPWKxJsvmwQiVBBxRLoxPTnXVaMU2jPV3MdFKZTobH",
      "hash": "ASS7oYwGiem9HaNwJe6vS2kznx2CxueKDvU9BAYJRjNR"
    },
    "transaction_outcome": {
      "proof": [],
      "block_hash": "9MzuZrRPW1BGpFnZJUJg6SzCrixPpJDfjsNeUobRXsLe",
      "id": "ASS7oYwGiem9HaNwJe6vS2kznx2CxueKDvU9BAYJRjNR",
      "outcome": {
        "logs": [],
        "receipt_ids": ["BLV2q6p8DX7pVgXRtGtBkyUNrnqkNyU7iSksXG7BjVZh"],
        "gas_burnt": 223182562500,
        "tokens_burnt": "22318256250000000000",
        "executor_id": "sender.testnet",
        "status": {
          "SuccessReceiptId": "BLV2q6p8DX7pVgXRtGtBkyUNrnqkNyU7iSksXG7BjVZh"
        }
      }
    },
    "receipts_outcome": [
      {
        "proof": [],
        "block_hash": "5Hpj1PeCi32ZkNXgiD1DrW4wvW4Xtic74DJKfyJ9XL3a",
        "id": "BLV2q6p8DX7pVgXRtGtBkyUNrnqkNyU7iSksXG7BjVZh",
        "outcome": {
          "logs": [],
          "receipt_ids": ["3sawynPNP8UkeCviGqJGwiwEacfPyxDKRxsEWPpaUqtR"],
          "gas_burnt": 223182562500,
          "tokens_burnt": "22318256250000000000",
          "executor_id": "receiver.testnet",
          "status": {
            "SuccessValue": ""
          }
        }
      },
      {
        "proof": [],
        "block_hash": "CbwEqMpPcu6KwqVpBM3Ry83k6M4H1FrJjES9kBXThcRd",
        "id": "3sawynPNP8UkeCviGqJGwiwEacfPyxDKRxsEWPpaUqtR",
        "outcome": {
          "logs": [],
          "receipt_ids": [],
          "gas_burnt": 0,
          "tokens_burnt": "0",
          "executor_id": "sender.testnet",
          "status": {
            "SuccessValue": ""
          }
        }
      }
    ]
  },
  "id": "11"
}
```