---
description: Queries status of a transaction by hash, returning the final transaction result and details of all receipts. 
---

# Transaction Status with Receipts

### **Parameters**

* `method:` EXPERIMENTAL_tx_status
* `params:` 
  * `transaction hash` 
  * `sender account id`

### **Returns**

Queries status of a transaction by hash, returning the final transaction result and details of all receipts.

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
  "method": "EXPERIMENTAL_tx_status",
  "params": ["BNTBdCWsNoSp7Kza8toTX7adbBFaGfk1cqdRbeaprSjd", "relay.aurora"]
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "receipts": [
            {
                "predecessor_id": "relay.aurora",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "FunctionCall": {
                                    "args": "+QGsgjprgIMPQkCUrtWyW+HDFjyQekcQgmQEUPko3f6AuQFEFzV4kgAAAAAAAAAAAAAAAPESybOJA0ZezIwFSbre7XLCtQcqAAAAAAAAAAAAAAAABzeVZc2LDK58YNx45/YBs0ryohwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAGmpUVcFuGks1aAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAArR2aKC1qwm/AAAAAAAAAAAAAAAAzvbC4giYwmBIhriIVSymzPZpM7AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAG+z/8CMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAYk2MwIt9yYiZS+1K4Dm1xO+JLswAsbDIyQxTOJiUBW84bbs9hJyKgsigg7uaJPPydxag1SV8IpF+V2Om5x9BHTyf5f1JGC8cpcWgcKH6Zxw4B4LapZD1ajaDEZ6rz5KNaLytQ5KaC3/oKro=",
                                    "deposit": "0",
                                    "gas": 300000000000000,
                                    "method_name": "submit"
                                }
                            }
                        ],
                        "gas_price": "625040174",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "relay.aurora",
                        "signer_public_key": "ed25519:74dWe1GfB9vn9aqfUnt6yuMQ2aKMw7hSewuwDB2LXeQJ"
                    }
                },
                "receipt_id": "DbhSVq1n33pdTa9R5XMGzCMxPEtAZJu59NkcC6EKBM35",
                "receiver_id": "aurora"
            },
            {
                "predecessor_id": "system",
                "receipt": {
                    "Action": {
                        "actions": [
                            {
                                "Transfer": {
                                    "deposit": "182849156714863146269492"
                                }
                            }
                        ],
                        "gas_price": "0",
                        "input_data_ids": [],
                        "output_data_receivers": [],
                        "signer_id": "relay.aurora",
                        "signer_public_key": "ed25519:74dWe1GfB9vn9aqfUnt6yuMQ2aKMw7hSewuwDB2LXeQJ"
                    }
                },
                "receipt_id": "HvSY52uknLFrsdubVmdg9MPE9zzbvwYxvnF9dznjF5TT",
                "receiver_id": "relay.aurora"
            }
        ],
        "receipts_outcome": [
            {
                "block_hash": "J4muLFEAa78HW4tYmRkaiS6yNjACxEgZK5ZqSCPZ3PqP",
                "id": "DbhSVq1n33pdTa9R5XMGzCMxPEtAZJu59NkcC6EKBM35",
                "outcome": {
                    "executor_id": "aurora",
                    "gas_burnt": 61810543781630,
                    "logs": [
                        "signer_address Address(0x230a1ac45690b9ae1176389434610b9526d2f21b)",
                        "total_writes_count 23",
                        "total_written_bytes 736"
                    ],
                    "metadata": {
                        "gas_profile": [
                            {
                                "cost": "BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "108025389288"
                            },
                            {
                                "cost": "CONTRACT_COMPILE_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "35445963"
                            },
                            {
                                "cost": "CONTRACT_COMPILE_BYTES",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "200471424750"
                            },
                            {
                                "cost": "ECRECOVER_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "278821988457"
                            },
                            {
                                "cost": "KECCAK256_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "17638473825"
                            },
                            {
                                "cost": "KECCAK256_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "9511699515"
                            },
                            {
                                "cost": "LOG_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "10629939150"
                            },
                            {
                                "cost": "LOG_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "1451867010"
                            },
                            {
                                "cost": "READ_MEMORY_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "482824692000"
                            },
                            {
                                "cost": "READ_MEMORY_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "32896735782"
                            },
                            {
                                "cost": "READ_REGISTER_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "317162813436"
                            },
                            {
                                "cost": "READ_REGISTER_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "17130075600"
                            },
                            {
                                "cost": "STORAGE_READ_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "7439103639000"
                            },
                            {
                                "cost": "STORAGE_READ_KEY_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "150584073045"
                            },
                            {
                                "cost": "STORAGE_READ_VALUE_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "971596014795"
                            },
                            {
                                "cost": "STORAGE_REMOVE_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "53473030500"
                            },
                            {
                                "cost": "STORAGE_REMOVE_KEY_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "2216782272"
                            },
                            {
                                "cost": "STORAGE_WRITE_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "1412328192000"
                            },
                            {
                                "cost": "STORAGE_WRITE_EVICTED_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "21582830304"
                            },
                            {
                                "cost": "STORAGE_WRITE_KEY_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "62588785896"
                            },
                            {
                                "cost": "STORAGE_WRITE_VALUE_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "21837051456"
                            },
                            {
                                "cost": "TOUCHING_TRIE_NODE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "28564869812724"
                            },
                            {
                                "cost": "UTF8_DECODING_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "9335337183"
                            },
                            {
                                "cost": "UTF8_DECODING_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "32073852690"
                            },
                            {
                                "cost": "WASM_INSTRUCTION",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "17255265842364"
                            },
                            {
                                "cost": "WRITE_MEMORY_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "350474357625"
                            },
                            {
                                "cost": "WRITE_MEMORY_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "473217252192"
                            },
                            {
                                "cost": "WRITE_REGISTER_BASE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "421231805442"
                            },
                            {
                                "cost": "WRITE_REGISTER_BYTE",
                                "cost_category": "WASM_HOST_COST",
                                "gas_used": "663266474208"
                            }
                        ],
                        "version": 1
                    },
                    "receipt_ids": [
                        "HvSY52uknLFrsdubVmdg9MPE9zzbvwYxvnF9dznjF5TT"
                    ],
                    "status": {
                        "SuccessValue": "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"
                    },
                    "tokens_burnt": "6181054378163000000000"
                },
                "proof": [
                    {
                        "direction": "Left",
                        "hash": "9kzRJqt7ZF5m7kNSHRJSPodex5zK5SMzcLX8jeKXZnQ9"
                    }
                ]
            },
            {
                "block_hash": "Ekv7tL1WSg1Xq1idRfbGJBpLwQMB4duNsaKQvFRHJgGV",
                "id": "HvSY52uknLFrsdubVmdg9MPE9zzbvwYxvnF9dznjF5TT",
                "outcome": {
                    "executor_id": "relay.aurora",
                    "gas_burnt": 223182562500,
                    "logs": [],
                    "metadata": {
                        "gas_profile": [],
                        "version": 1
                    },
                    "receipt_ids": [],
                    "status": {
                        "SuccessValue": ""
                    },
                    "tokens_burnt": "0"
                },
                "proof": [
                    {
                        "direction": "Left",
                        "hash": "6EP6RWfJSUJcxU37aAyXUnJtN999c7rdpctRKCay3A7E"
                    },
                    {
                        "direction": "Right",
                        "hash": "AP8BVzrPXDG9ts3Xr1gkSTiBZYHUWeSA3FzV8ZNZiPmE"
                    },
                    {
                        "direction": "Left",
                        "hash": "7HdXeLsnjmqC1QzzWRvQxfdMxcV6AT7yxzAYwqPaePce"
                    },
                    {
                        "direction": "Right",
                        "hash": "8bn3LNnVLxY3PoepTs3pHgdS8NcTTgpNw4ujW4hoG4Gc"
                    }
                ]
            }
        ],
        "status": {
            "SuccessValue": "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"
        },
        "transaction": {
            "actions": [
                {
                    "FunctionCall": {
                        "args": "+QGsgjprgIMPQkCUrtWyW+HDFjyQekcQgmQEUPko3f6AuQFEFzV4kgAAAAAAAAAAAAAAAPESybOJA0ZezIwFSbre7XLCtQcqAAAAAAAAAAAAAAAABzeVZc2LDK58YNx45/YBs0ryohwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAGmpUVcFuGks1aAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAArR2aKC1qwm/AAAAAAAAAAAAAAAAzvbC4giYwmBIhriIVSymzPZpM7AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAG+z/8CMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAYk2MwIt9yYiZS+1K4Dm1xO+JLswAsbDIyQxTOJiUBW84bbs9hJyKgsigg7uaJPPydxag1SV8IpF+V2Om5x9BHTyf5f1JGC8cpcWgcKH6Zxw4B4LapZD1ajaDEZ6rz5KNaLytQ5KaC3/oKro=",
                        "deposit": "0",
                        "gas": 300000000000000,
                        "method_name": "submit"
                    }
                }
            ],
            "hash": "BNTBdCWsNoSp7Kza8toTX7adbBFaGfk1cqdRbeaprSjd",
            "nonce": 59304131020958,
            "public_key": "ed25519:74dWe1GfB9vn9aqfUnt6yuMQ2aKMw7hSewuwDB2LXeQJ",
            "receiver_id": "aurora",
            "signature": "ed25519:3839GmXyMqGekPp5S2a5tE7rWZq4uEALbNitfRN4hLUjnbD8SgoVpYcZjnrkSNquJCMbHg6khTfofQ51zrifzLy3",
            "signer_id": "relay.aurora"
        },
        "transaction_outcome": {
            "block_hash": "DwszNfJLgNkSvBa21z5LbLPrGGzp29a5muUKhREccShu",
            "id": "BNTBdCWsNoSp7Kza8toTX7adbBFaGfk1cqdRbeaprSjd",
            "outcome": {
                "executor_id": "relay.aurora",
                "gas_burnt": 2428898103158,
                "logs": [],
                "metadata": {
                    "gas_profile": null,
                    "version": 1
                },
                "receipt_ids": [
                    "DbhSVq1n33pdTa9R5XMGzCMxPEtAZJu59NkcC6EKBM35"
                ],
                "status": {
                    "SuccessReceiptId": "DbhSVq1n33pdTa9R5XMGzCMxPEtAZJu59NkcC6EKBM35"
                },
                "tokens_burnt": "242889810315800000000"
            },
            "proof": [
                {
                    "direction": "Right",
                    "hash": "HrXU3yLhMvv56xMkPK9ZdoSdSRhHrEnZK3rcPkVBgGff"
                },
                {
                    "direction": "Right",
                    "hash": "GChWQCavwhVBnMDqxphANxuGbgY4dj9FYFZzf53ovZXd"
                },
                {
                    "direction": "Left",
                    "hash": "GhfwKEpCTRxdnH1HrSrApcCJbN2iMnPiET3ECaEyF9oK"
                },
                {
                    "direction": "Right",
                    "hash": "9jBU8FnLDWF5wRpLQBh3G7NHuKhsUuuCdXNBULXeS6d7"
                }
            ]
        }
    }
}
```