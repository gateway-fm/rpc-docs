---
description: Returns details of a specific chunk.
---

# Chunk Details

### **Parameters**

* `method:` chunk
* `params:`
  * `chunk_id` OR `block_id`, `shard_id`

### **Returns**

Returns details of a specific chunk. You can run a block details query to get a valid chunk hash.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v1/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "dontcare",
  "method": "chunk",
  "params": {"block_id": 62888150, "shard_id": 0}
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "dontcare",
    "result": {
        "author": "pathrocknetwork.poolv1.near",
        "header": {
            "balance_burnt": "1694749035665800000000",
            "chunk_hash": "F6gDNte9pyockVAXXx9PaFZQrbMNEdETSfJicgZVtwY6",
            "encoded_length": 1116,
            "encoded_merkle_root": "27Nmn4RJDx6wiVkU2U7YhEkhJxvdZPDEbgAJUXzvRSWf",
            "gas_limit": 1000000000000000,
            "gas_used": 19453831570632,
            "height_created": 62888150,
            "height_included": 62888150,
            "outcome_root": "158ub1BMSiUvRTMgcDwnqzXJR7Hn7Q8GG453typvPPA",
            "outgoing_receipts_root": "3vEUinNcZKc6Mgb4mhAncCNncpkAj4bBV9yzsGgahNzo",
            "prev_block_hash": "E7oLDgVwcPaL843bKBA8JFSKHvHwZjeT5r6wqtDxW9kW",
            "prev_state_root": "EUwsuDcWn9yW3S7RB4rB2R29cGAcmo1URRzaAY8M62z9",
            "rent_paid": "0",
            "shard_id": 0,
            "signature": "ed25519:2djKGUMFabxEweFKFPdpnMejKt2yR9j8vDMdPiVaA7txpdDsLgG1fPG97jxz75rNj763EtuVDsaQBBmREunBMQR4",
            "tx_root": "Ev6kaAtw7uAHBsNb1ko6iEcY6phfsVaDpfgcxquS7nGa",
            "validator_proposals": [],
            "validator_reward": "0"
        },
        "receipts": [
            {
                "predecessor_id": "system",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "Transfer": {
                                    "deposit": "67637586630767327711160"
                                }
                            }
                        ],
                        "gas_price": "0",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "app.nearcrowd.near",
                        "signer_public_key": "ed25519:HtW1yGPW7JUAorCgJvjQyank8nWHHgXC2dMLxyA7YCuW"
                    }
                },
                "receipt_id": "6Te2RuuyMVcKVTtdH37yixJGm2vjdS5DDpUXv1UD6AFa",
                "receiver_id": "app.nearcrowd.near"
            },
            {
                "predecessor_id": "system",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "Transfer": {
                                    "deposit": "13011914738233142651168"
                                }
                            }
                        ],
                        "gas_price": "0",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "marii.near",
                        "signer_public_key": "ed25519:EvFtS4LMFiTPtk6ZDN5Z86VVi4za8GvroXr5bMzFzq6k"
                    }
                },
                "receipt_id": "BbYyFnzw7UpTjUSYbVXdvvWjFQ1tNF34U42tav1hAssg",
                "receiver_id": "marii.near"
            },
            {
                "predecessor_id": "system",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "Transfer": {
                                    "deposit": "3649464383448273249404"
                                }
                            }
                        ],
                        "gas_price": "0",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "makaron.near",
                        "signer_public_key": "ed25519:FKJV4cXSGnJoegeteYK4zEp7dxR8YUkoykuB9DXppY43"
                    }
                },
                "receipt_id": "FUPbMNX37k6YRfu42YjKVk7zAnDjfL3R1jhMKrACQ9vn",
                "receiver_id": "makaron.near"
            },
            {
                "predecessor_id": "system",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "Transfer": {
                                    "deposit": "3023456692785595595520"
                                }
                            }
                        ],
                        "gas_price": "0",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "biidrii.near",
                        "signer_public_key": "ed25519:2BXFDeFqo8GzuMKZxAbvNVp8vzK9PhUPjmsnhAMvhYcK"
                    }
                },
                "receipt_id": "GHnuSrmJDLSnoE3BF1ZgjJYjfAYSJUCSGAxqaV8RsLai",
                "receiver_id": "biidrii.near"
            }
        ],
        "transactions": [
            {
                "actions": [
                    {
                        "FunctionCall": {
                            "args": "eyJ0YXNrX29yZGluYWwiOjEsImlzX2hvbmV5cG90IjpmYWxzZSwiaG9uZXlwb3RfcHJlaW1hZ2UiOls5OCwxMTcsMTEyLDEwMSwxMDcsMTE3LDExNywxMDksMTEzLDEwMSwxMjEsMTE4LDEwNSwxMDgsMTA0LDk4XSwidGFza19wcmVpbWFnZSI6WzI0MSwyMSwxNDYsMjMwLDk3LDIxMCw3OSwxMjYsMTg4LDY1LDIxMCwxMjMsMjA2LDQ3LDYxLDEwOSwxMTYsNDIsMTQ1LDQ4LDM3LDE4MSwyMzYsMjQyLDkzLDE0OSw4MywyMjMsNDgsMTI2LDI0NywxMDVdfQ==",
                            "deposit": "0",
                            "gas": 200000000000000,
                            "method_name": "finalize_task"
                        }
                    }
                ],
                "hash": "67DbMWEvrzbM3jXjPx1buXaPDWgPvbX3rcKWWBMSvbap",
                "nonce": 42863155352886,
                "public_key": "ed25519:6MP4bCPHEud33eKXM9kg7f9fVNhmn97CNUyn5ZwM375U",
                "receiver_id": "app.nearcrowd.near",
                "signature": "ed25519:343eqXV2oSM22J8X2jQsb3KARfDXcGJVmSAg333UCdo7zxBuEyKHhzLGoYvPyoks5ZsjRwj7UC3P3jiSDCLGC2f5",
                "signer_id": "app.nearcrowd.near"
            }
        ]
    }
}
```