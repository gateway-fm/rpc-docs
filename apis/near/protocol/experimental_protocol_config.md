---
description: Returns most recent protocol configuration or a specific queried block. 
---

# Protocol Config

### **Parameters**
* `method:` EXPERIMENTAL_protocol_config
* `params:` 
  * `finality` OR `block_id`

### **Returns**
Returns most recent protocol configuration or a specific queried block. Useful for finding current storage and transaction costs.

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
  "method": "EXPERIMENTAL_protocol_config",
  "params": {
    "finality": "final"
  }
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "avg_hidden_validator_seats_per_shard": [
            0,
            0,
            0,
            0
        ],
        "block_producer_kickout_threshold": 90,
        "chain_id": "mainnet",
        "chunk_producer_kickout_threshold": 90,
        "dynamic_resharding": false,
        "epoch_length": 43200,
        "fishermen_threshold": "340282366920938463463374607431768211455",
        "gas_limit": 1000000000000000,
        "gas_price_adjustment_rate": [
            1,
            100
        ],
        "genesis_height": 9820210,
        "genesis_time": "2020-07-21T16:55:51.591948Z",
        "max_gas_price": "10000000000000000000000",
        "max_inflation_rate": [
            0,
            1
        ],
        "min_gas_price": "1000000000",
        "minimum_stake_divisor": 10,
        "num_block_producer_seats": 100,
        "num_block_producer_seats_per_shard": [
            100,
            100,
            100,
            100
        ],
        "num_blocks_per_year": 31536000,
        "online_max_threshold": [
            99,
            100
        ],
        "online_min_threshold": [
            90,
            100
        ],
        "protocol_reward_rate": [
            0,
            1
        ],
        "protocol_treasury_account": "treasury.near",
        "protocol_upgrade_stake_threshold": [
            4,
            5
        ],
        "protocol_version": 52,
        "runtime_config": {
            "account_creation_config": {
                "min_allowed_top_level_account_length": 32,
                "registrar_account_id": "registrar"
            },
            "storage_amount_per_byte": "10000000000000000000",
            "transaction_costs": {
                "action_creation_config": {
                    "add_key_cost": {
                        "full_access_cost": {
                            "execution": 101765125000,
                            "send_not_sir": 101765125000,
                            "send_sir": 101765125000
                        },
                        "function_call_cost": {
                            "execution": 102217625000,
                            "send_not_sir": 102217625000,
                            "send_sir": 102217625000
                        },
                        "function_call_cost_per_byte": {
                            "execution": 1925331,
                            "send_not_sir": 1925331,
                            "send_sir": 1925331
                        }
                    },
                    "create_account_cost": {
                        "execution": 99607375000,
                        "send_not_sir": 99607375000,
                        "send_sir": 99607375000
                    },
                    "delete_account_cost": {
                        "execution": 147489000000,
                        "send_not_sir": 147489000000,
                        "send_sir": 147489000000
                    },
                    "delete_key_cost": {
                        "execution": 94946625000,
                        "send_not_sir": 94946625000,
                        "send_sir": 94946625000
                    },
                    "deploy_contract_cost": {
                        "execution": 184765750000,
                        "send_not_sir": 184765750000,
                        "send_sir": 184765750000
                    },
                    "deploy_contract_cost_per_byte": {
                        "execution": 6812999,
                        "send_not_sir": 6812999,
                        "send_sir": 6812999
                    },
                    "function_call_cost": {
                        "execution": 2319861500000,
                        "send_not_sir": 2319861500000,
                        "send_sir": 2319861500000
                    },
                    "function_call_cost_per_byte": {
                        "execution": 2235934,
                        "send_not_sir": 2235934,
                        "send_sir": 2235934
                    },
                    "stake_cost": {
                        "execution": 102217625000,
                        "send_not_sir": 141715687500,
                        "send_sir": 141715687500
                    },
                    "transfer_cost": {
                        "execution": 115123062500,
                        "send_not_sir": 115123062500,
                        "send_sir": 115123062500
                    }
                },
                "action_receipt_creation_config": {
                    "execution": 108059500000,
                    "send_not_sir": 108059500000,
                    "send_sir": 108059500000
                },
                "burnt_gas_reward": [
                    3,
                    10
                ],
                "data_receipt_creation_config": {
                    "base_cost": {
                        "execution": 36486732312,
                        "send_not_sir": 36486732312,
                        "send_sir": 36486732312
                    },
                    "cost_per_byte": {
                        "execution": 17212011,
                        "send_not_sir": 17212011,
                        "send_sir": 17212011
                    }
                },
                "pessimistic_gas_price_inflation_ratio": [
                    103,
                    100
                ],
                "storage_usage_config": {
                    "num_bytes_account": 100,
                    "num_extra_bytes_record": 40
                }
            },
            "wasm_config": {
                "ext_costs": {
                    "base": 264768111,
                    "contract_compile_base": 35445963,
                    "contract_compile_bytes": 216750,
                    "ecrecover_base": 278821988457,
                    "keccak256_base": 5879491275,
                    "keccak256_byte": 21471105,
                    "keccak512_base": 5811388236,
                    "keccak512_byte": 36649701,
                    "log_base": 3543313050,
                    "log_byte": 13198791,
                    "promise_and_base": 1465013400,
                    "promise_and_per_promise": 5452176,
                    "promise_return": 560152386,
                    "read_memory_base": 2609863200,
                    "read_memory_byte": 3801333,
                    "read_register_base": 2517165186,
                    "read_register_byte": 98562,
                    "ripemd160_base": 853675086,
                    "ripemd160_block": 680107584,
                    "sha256_base": 4540970250,
                    "sha256_byte": 24117351,
                    "storage_has_key_base": 54039896625,
                    "storage_has_key_byte": 30790845,
                    "storage_iter_create_from_byte": 0,
                    "storage_iter_create_prefix_base": 0,
                    "storage_iter_create_prefix_byte": 0,
                    "storage_iter_create_range_base": 0,
                    "storage_iter_create_to_byte": 0,
                    "storage_iter_next_base": 0,
                    "storage_iter_next_key_byte": 0,
                    "storage_iter_next_value_byte": 0,
                    "storage_read_base": 56356845750,
                    "storage_read_key_byte": 30952533,
                    "storage_read_value_byte": 5611005,
                    "storage_remove_base": 53473030500,
                    "storage_remove_key_byte": 38220384,
                    "storage_remove_ret_value_byte": 11531556,
                    "storage_write_base": 64196736000,
                    "storage_write_evicted_byte": 32117307,
                    "storage_write_key_byte": 70482867,
                    "storage_write_value_byte": 31018539,
                    "touching_trie_node": 16101955926,
                    "utf16_decoding_base": 3543313050,
                    "utf16_decoding_byte": 163577493,
                    "utf8_decoding_base": 3111779061,
                    "utf8_decoding_byte": 291580479,
                    "validator_stake_base": 911834726400,
                    "validator_total_stake_base": 911834726400,
                    "write_memory_base": 2803794861,
                    "write_memory_byte": 2723772,
                    "write_register_base": 2865522486,
                    "write_register_byte": 3801564
                },
                "grow_mem_cost": 1,
                "limit_config": {
                    "initial_memory_pages": 1024,
                    "max_actions_per_receipt": 100,
                    "max_arguments_length": 4194304,
                    "max_contract_size": 4194304,
                    "max_functions_number_per_contract": 10000,
                    "max_gas_burnt": 300000000000000,
                    "max_length_method_name": 256,
                    "max_length_returned_data": 4194304,
                    "max_length_storage_key": 4194304,
                    "max_length_storage_value": 4194304,
                    "max_memory_pages": 2048,
                    "max_number_bytes_method_names": 2000,
                    "max_number_input_data_dependencies": 128,
                    "max_number_logs": 100,
                    "max_number_registers": 100,
                    "max_promises_per_function_call_action": 1024,
                    "max_register_size": 104857600,
                    "max_stack_height": 16384,
                    "max_total_log_length": 16384,
                    "max_total_prepaid_gas": 300000000000000,
                    "max_transaction_size": 4194304,
                    "registers_memory_limit": 1073741824,
                    "stack_limiter_version": 1
                },
                "regular_op_cost": 822756
            }
        },
        "transaction_validity_period": 86400
    }
}
```