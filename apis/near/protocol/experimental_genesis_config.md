---
description: Returns current genesis configuration.


---

# Gas Price

### **Parameters**
* `method:` EXPERIMENTAL_genesis_config
* `params:` none

### **Returns**
Returns current genesis configuration.

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
  "method": "EXPERIMENTAL_genesis_config"
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "avg_hidden_validator_seats_per_shard": [
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
        "minimum_stake_ratio": [
            1,
            6250
        ],
        "num_block_producer_seats": 100,
        "num_block_producer_seats_per_shard": [
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
        "protocol_upgrade_num_epochs": 2,
        "protocol_upgrade_stake_threshold": [
            4,
            5
        ],
        "protocol_version": 29,
        "shard_layout": {
            "V0": {
                "num_shards": 1,
                "version": 0
            }
        },
        "simple_nightshade_shard_layout": {
            "V1": {
                "boundary_accounts": [
                    "aurora",
                    "aurora-0",
                    "kkuuue2akv_1630967379.near"
                ],
                "fixed_shards": [],
                "shards_split_map": [
                    [
                        0,
                        1,
                        2,
                        3
                    ]
                ],
                "to_parent_shard_map": [
                    0,
                    0,
                    0,
                    0
                ],
                "version": 1
            }
        },
        "total_supply": "999999999792372916156395166000000",
        "transaction_validity_period": 86400,
        "validators": [
            {
                "account_id": "nfvalidator1.near",
                "amount": "50000000000000000000000000000",
                "public_key": "ed25519:14pWWRutZtGFKX4B8q89KVFaUWY1Cqu1JcqYXhCDeFh1"
            },
            {
                "account_id": "nfvalidator2.near",
                "amount": "50000000000000000000000000000",
                "public_key": "ed25519:BwZk4bkYJxo79P2vSRw2uk1nfiqEfVkHvr5p8eVsqASC"
            },
            {
                "account_id": "nfvalidator3.near",
                "amount": "50000000000000000000000000000",
                "public_key": "ed25519:DMz11tmPvhdqpi7CzP2JULeeSE8SxYRD8pys5nKke4FS"
            },
            {
                "account_id": "nfvalidator4.near",
                "amount": "50000000000000000000000000000",
                "public_key": "ed25519:Fi3CQDHJoviKazVR27YmfFzWcFnvmoPBKEDd9ouq5Tjx"
            }
        ]
    }
}
```