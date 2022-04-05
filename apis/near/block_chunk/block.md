---
description: Queries network and returns block for given height or hash.
---

# Block details

### **Parameters**
* `method:` block
* `params:`
  * `finality` OR `block_id`

### **Returns**
Queries network and returns block for given height or hash. You can also use finality param to return latest block details.

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
  "method": "block",
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
        "author": "node0",
        "chunks": [
            {
                "balance_burnt": "0",
                "chunk_hash": "8BjNvg1X3mru84CPgqvRuvBqirqMSbhXeb8sTk7PmyTM",
                "encoded_length": 8,
                "encoded_merkle_root": "5TxYudsfZd2FZoMyJEZAP19ASov2ZD43N8ZWv8mKzWgx",
                "gas_limit": 1000000000000000,
                "gas_used": 0,
                "height_created": 86800609,
                "height_included": 86800609,
                "outcome_root": "11111111111111111111111111111111",
                "outgoing_receipts_root": "8s41rye686T2ronWmFE38ji19vgeb6uPxjYMPt8y8pSV",
                "prev_block_hash": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
                "prev_state_root": "FgccVBRpyno1eEV2kbu15vKLAruiFiL5trZAnk2dKdcC",
                "rent_paid": "0",
                "shard_id": 0,
                "signature": "ed25519:3adp8az23Cn47exoGctkxGw2jyBKvbCexghtWughvMcmaLeswD3tv955N6fViYxeXLRMKGKc2tGJ44JqFDpZ8NWA",
                "tx_root": "11111111111111111111111111111111",
                "validator_proposals": [],
                "validator_reward": "0"
            },
            {
                "balance_burnt": "381288092034800000000",
                "chunk_hash": "6EZDFWGR8VC7gMzJxpYf4ZETqERS3Vxou9LJoVtpXK2w",
                "encoded_length": 161,
                "encoded_merkle_root": "29dUUn3XdcSdf9b5QRwdFzxrx4fcNS3Pot1ea3epDoxZ",
                "gas_limit": 1000000000000000,
                "gas_used": 4406290475053,
                "height_created": 86800609,
                "height_included": 86800609,
                "outcome_root": "9MFnwL9Yvmk4vfBn4GyhBVfDEDQFP5dH5oK3WkcYMKfe",
                "outgoing_receipts_root": "DmQ7p5z8VysZJK4gbJEzECttTaa1SphaDJE6idJHVzg4",
                "prev_block_hash": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
                "prev_state_root": "9tfSpRhzbrCHffR2WYyJz39cakpv1v8Zg4ntQrezUpRF",
                "rent_paid": "0",
                "shard_id": 1,
                "signature": "ed25519:3r1iBZDvW6xbz9hB631wHGMUkHR1NxiT1ZykGmLJSj7waGMQGqPM6pEWYYkdiy5JwPTL8ivQi4bR9JCLfcQdjbdc",
                "tx_root": "11111111111111111111111111111111",
                "validator_proposals": [],
                "validator_reward": "0"
            },
            {
                "balance_burnt": "0",
                "chunk_hash": "6C1y8GaUDwsEasJ7bpuH6kAhrXVYambUzMTSZFKdtxRe",
                "encoded_length": 583,
                "encoded_merkle_root": "FrEomcqVhAVbHomMFnynTrANPF5YMTrCr412XgG5xbPb",
                "gas_limit": 1000000000000000,
                "gas_used": 0,
                "height_created": 86800609,
                "height_included": 86800609,
                "outcome_root": "11111111111111111111111111111111",
                "outgoing_receipts_root": "8s41rye686T2ronWmFE38ji19vgeb6uPxjYMPt8y8pSV",
                "prev_block_hash": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
                "prev_state_root": "3e8nuBkxUm1Re41UBC3ooMXnPRJDPUond6YY75Wqe9aD",
                "rent_paid": "0",
                "shard_id": 2,
                "signature": "ed25519:4vcYiSWH9d6h3Yi5Xv5QTWUvodLYQhwqKxVYKFkHAg7LTUK7kQm675nCfSEfvzdLxfzWB5tcnKhR68Wzg8HiY6ta",
                "tx_root": "FpaJterXzbqAXqwsbUNsB6jpNDq9SCfarxxEJHksqezg",
                "validator_proposals": [],
                "validator_reward": "0"
            },
            {
                "balance_burnt": "1192211305985300000000",
                "chunk_hash": "B3idw8Mwr4LTvMXX8rGk1U7n12TgCZxPVZX5zhBXRosg",
                "encoded_length": 2800,
                "encoded_merkle_root": "6RefcTeGW981DzvaLQERzF8mzq3ABQsd6aougwP78Eo8",
                "gas_limit": 1000000000000000,
                "gas_used": 14356114430949,
                "height_created": 86800609,
                "height_included": 86800609,
                "outcome_root": "B1yYvrnLrNM5EGEQo2eUGYTL1h5Gt6KwR4ERmNbA3B1",
                "outgoing_receipts_root": "8GSVc4t2Y9Z6KTAQmfeD7soqmmzoHhftb7SuSC6tfEL2",
                "prev_block_hash": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
                "prev_state_root": "Ek9HfN2ji8DTFw2Ts4gvk4iZxukYVBAeyJyPjfPJivtG",
                "rent_paid": "0",
                "shard_id": 3,
                "signature": "ed25519:3LCE3h2fgZxiLYVBeAnaxeFmVCB3fDXz2edZsXmkzyotoMERUQckhpq7Rr2yaLcdBo3ei7AjhReUrkK6xzCWRKFh",
                "tx_root": "7FHrYTna9ZyUvbJFhnLe8DpBoja574g6tUfHhnbsLf2q",
                "validator_proposals": [],
                "validator_reward": "0"
            }
        ],
        "header": {
            "approvals": [
                "ed25519:SMFw48iUiQBPo44zjgdJ1zbk2Ec1FrocK1YiyLafPd6yA1UKXD7YviNEyT4tnx5Xy1ADRwH8NvtXMvNJXU3bqTD",
                "ed25519:SMFw48iUiQBPo44zjgdJ1zbk2Ec1FrocK1YiyLafPd6yA1UKXD7YviNEyT4tnx5Xy1ADRwH8NvtXMvNJXU3bqTD",
                null,
                "ed25519:SMFw48iUiQBPo44zjgdJ1zbk2Ec1FrocK1YiyLafPd6yA1UKXD7YviNEyT4tnx5Xy1ADRwH8NvtXMvNJXU3bqTD",
                "ed25519:b58Us87T1ciGinV8GoH3bpvF8ZXjueNCsvsScBcwkKwC3MD8Lbt62icwp6Ud7q6bf6NcPMyPk2jAYizqJmcszQK",
                "ed25519:5Pyp7dinZMeoSqJRhqgFdWUcRCH9oM4hs1dkRhd2Cxqf8pLGvGFFkYyT58Y2o34WWiwJod5LA5wRbAawXqDqrTF6",
                "ed25519:5Xkza1mfj7WUkUHv6m4nwDu9KJiaWHKrd6WzXRJ5MNwSBJbZrYkvdcFT6J9GPHdVoNNyPz6uwdocfgpJBjy1a4Nr",
                "ed25519:5aCb2LmeKjWD5z8QPaYVJwhNCw7ofDKoPR1B1a44mzWVBNLJTiY6ySmtQJLzuQcmCtqifN9fhM5nWigmDfTnuLak",
                "ed25519:22J2uj7nFFxXXnU4MpEJN53q8G2JJ6dV1mabqhmBE17iAr1NmviQ8zm9SJrQBJd3ZULt6GgqicxWCJRmZafe4Mo6",
                null,
                "ed25519:mfT6zNWHeegbZeCzsXd4nUF42LgKcf4dvBCyVq6VmUz6KaR4rncNNjHZu4sgY9XmiR4pfUjSx3faVWrytSbSQs9",
                "ed25519:4VBfYAhY9baLrei7vbJPiriTD7yXE8X8jQ2bfqqeUDWCPz9xCfq5EcPJzAQvnakWoAJ9T4fMczDsvV1L6SgTatuk",
                null,
                null,
                "ed25519:3h8vMH4hxYtPQwoVJ1fuAXT3jNuCrce2XMotLbw5nThAyaDqGsGc1evfzuwgYHumjrytfUXdXHtoh7auhSdg8Z21",
                "ed25519:4QksK2up8YmfaPgotVrRhiwVaYfBT7AM4itAL62EcjZcF63smpfpvS5JhxTMQdULT7j5eWZ7SMvnAhK5Dt9xzJy",
                "ed25519:pDj6XvSdX8hhMg7o5kpegZdzFND6mrMDqzGxWdqG1JvpLS1Lv7b6Kwy7Z64pFWtiaCuM1WAEbUGFA5fWrzZ2f1a",
                "ed25519:2b3EiqrCE3REzFsEA1vnq5KiVfz3VqseAW3xf2yeJwrgfEiVcMxafoQkt5s4kx8jndctu3rhTvS8BQHvBzRFgzX6",
                "ed25519:2hkWUBujvPkNSqBhLPdJrA9m6MN2z2fo87KWDoAPEPq2AmR6eyVF3o1AB1iswvRfEekq3DwJ2AubUeBV3d3Y7BRM",
                "ed25519:2Eiq5G3ytSQmh25akL3VrBYL277ScXReXDSvtSmcgTAYGfavMEJqCk8cYmVzBZ3xzKes35b9gYsNuwSoCh83R5Mx",
                null,
                "ed25519:3zTnwFF3HqLEEwm1N8i8VPrW3goDPd8ikUdmM54uHow2TW1mMobaR9GTwBNvfS1mRryGxtDqHPX1o7J6u92mdqQK",
                "ed25519:HPwhPe6VAMthGrFPC1fQkBS9F1ibB4fTBRmdmQfP2WU7iQWR7K8ZhRiKdsASA48kgD1Q2yeN8UckggZNpypWLCi",
                null,
                "ed25519:4Ch5yEELEKr6jV542vmh5B5x2o6EZx829Z1pZx52FRoJ69aEqCzPBTDYmtdk3vNUJUdSGY7PPpbaT4cMsBBKgi2C",
                "ed25519:5EiS1Qkra2TZjwVYMASggTPdpW2xuSLGpoxYLna1Yw88MHFgntbGpBG2Hf4pbPqaBKiGpDEionFu1vJ3jjaUgvMh",
                "ed25519:4TXmV1skEw4Fn6jxLgiwWszyjGf3w5THqG6KRxJyWEXk3yZs6qFBxDZ6bX9fBozd9Ltwnhf7AEVsnGXJg9a9NSMU",
                "ed25519:2Mnvyd3eAQfzVVD4XhxD6h4WR9ZySE33nCNASSZeaRy4SxVqYSkLwkizK5uSmPphmeh7awoav9675PfgMU52VXK8",
                "ed25519:4npX4HAVDpxN6d2UHSenvQ1VzBn5gN4D4Sn4dU2mEm4Q4JyYTXiZ8t6mkLX3qxUVeD5ucZhp8ratJ7iysdfmciUi",
                "ed25519:7BFyVJoXe9uurkP9UnRum4MdRo21fbpy5U7umicibXg1mYPzBi6hv3gNk2DKnJMHViEeTxoZ9GRS1LG3WSkswEY",
                "ed25519:2Nez8gJVatwvVMfvWcx8BgVcwKkDsZXgmkH5TRfjDTmhXGZcJQcTbq3po5RqtE4PTfZGybJfuPN9KvgheC6NyTNm",
                "ed25519:35xTDV1CfufSGD2ePMPKEPu8aBjhtpKC63ypYKZcEuWHucCzw1F6sBEP7UnEw7KgBNBq7Wksg1CtJGaGSiXTUv6L",
                "ed25519:3pUdRfNGPbYRNbWHYKGWVKbdf735W2Xz7zqLjrqdhm89Ga8kfuLfrTcwwbEQnV3RPTz17sMrT1ZkmuuvTfsQvzaN",
                "ed25519:2h1y32nzmymoHSJvvnLPfz2doHL3sQoY2L4SC4SjNYhcxtV4b3VCFsMarVuhDdwFc8R7Yu1SBFCw9ayQLNAiumpT",
                "ed25519:4AB9E1mDnwmfBJBaZZ35QxHXEYwDJBnr5aWpfy21igis8Wm3iWwJaVYGXXiB6WUYYp1eJWyKmFT9nF9BEeVD1nju",
                null,
                "ed25519:5gSu73SbWUCjsuCAYtDusYQFGAPGUcxUDezmaJKjmVWVffwwG1P4ZasfiDqSybrYX1aeGYzRPt9twDrWo7gWZ4bs",
                null,
                "ed25519:2RF1FHPf33RwbJehJj357cFGqtNbBNHvZjzz8z1LiGZC2LMLLNXM82G4ZEQoCrzDvX6i3cnPvJgL1Lpw1iXvQNEt",
                null,
                "ed25519:4uVpJthJsHsPqjBqTuAAfh1Gfj2rD1LCLV4BgBbe81J2hxUxbmm3WmnYZc6xH1NuVrwo5w6iz5RTyzRB2iBFoyAD",
                "ed25519:5dmWNbrMXy4ktYDiUsWXyuKj1ysq3gCuyjtSjfLKcpGEs9xo9Chzx5mRVx11fxhXhA8CpxYhYE2Qp4x3vpFyHz5Q",
                "ed25519:2Ctfv2xCK5S5wwAWRdmnZwXT5R7fBuAm1Keq1omfUwpaRw4BfWUEA7MhKZHdYQ3ToGSYbb6uLPHwRFqezBADpAmN",
                "ed25519:2jDpBWirTvuX8ZWw52etr4xkFpfTnNCPTT7SawNxLkeJnTpy7oeSY1VACRJuDxiLqwowH2yDQ8chdLEcd2tppfrh",
                "ed25519:X7Znra3HXt9z2AdiWquiPbZ4MbgCWx6kia6DNLPKKMTh6Y5YPpVYu1BV8jsMNt9degRknfxmQtoTtxxZk3KjsFX",
                null,
                null,
                "ed25519:nXMGrLPtgGdsuikzHb8ihgAtGZQubJG3nH9WBhvRrkSxJHyzb1ik1Cpc49WoVq41i78bguCwmVFdrbbqoVyGQbz",
                null,
                null,
                "ed25519:aRLbDSkvKy8Fw5R8sz2pXNZBE1Wgzo34z3cYqcC2AvD9b2HUsFAzc4AMphcJsxjVxcfp2WGa2MRhYB6thfhsGsF",
                null,
                null,
                null,
                null,
                null,
                null,
                "ed25519:64yWTVXWyGbU1R9qTekZwEbh45ZTQSWzZLn9qxisFxLHYRRPRFt7BLV7u5N34tAGYaU2jG8KGaxc5u1cdrR56rSw",
                "ed25519:2BhRenK8zFtR4r5GqeB6z4aEnBrZ5BvmpAdZ2n3TCrPkfwd46uEBzEMhzAB5WgiPoDFCZUKS9FJvmiZ35waZohEi",
                null,
                "ed25519:XyuqgLms4Ga83wmau2Wu5wsx9ibmAK7nENMNED5CJxoDrtrQm7cyAkdTKGfy3wRcvhDVWNmjw4zqpz2hVGSz95p",
                "ed25519:673NzSLDwsmfPkDgyd6NPaDpeRHrzLqYEuAUprgsWWfFFn6jnSG984xFvTPRMQfZPcMogPqMVWaDspyMaXx23uTT",
                null,
                "ed25519:57NkUTcEgmjrz2pjTHmScctXSxYmRGkDUuPfFXa27x4MSbSwFJpkK6R4RHEp9mB5DMn8y8hud7rkSfTKWqBJsVZx",
                null,
                null,
                null,
                "ed25519:5E2PBzKS4Hrs1JjCbf1bFSDsPThvS5bS3XmcJXfxqDy4LeAaHhuDxWsG22oUAkNAn2vREdo6Bnz64cpkfyiFZBPf",
                "ed25519:3Df3VMU98HaaFgCdkQub8A3whiz6ZGqi4fqmPbBvQnM7cBzow7ZfzRjSE32P27ZFEKQqfepfhPjpu4CsczkRs2E3"
            ],
            "block_merkle_root": "6t79swWCECqNzVo4PTCdFJfqJRaLJFqxGLC63QFps6fL",
            "block_ordinal": 42387139,
            "challenges_result": [],
            "challenges_root": "11111111111111111111111111111111",
            "chunk_headers_root": "B5H1hdo6vqKS19TWn3dC4Gty11Nt1wB3sUyq3stU6Yvu",
            "chunk_mask": [
                true,
                true,
                true,
                true
            ],
            "chunk_receipts_root": "J54C43uNxUBy9UrQ2Y46Xe5feHS93NiiK6XtbELAgn4D",
            "chunk_tx_root": "4WHnz5By57twsRt153WGSLXZ9Bgsr5gRvhYD5t1Mjmhp",
            "chunks_included": 4,
            "epoch_id": "FWKCjBUvsB25QKj8GR898M7JSSrXDMD9dhBAVBeo9UyZ",
            "epoch_sync_data_hash": null,
            "gas_price": "100000000",
            "hash": "7AkeqKKZszLhHcKU9rQHAVpD5pxDUGRiQsPDYqKt6f6n",
            "height": 86800609,
            "last_ds_final_block": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
            "last_final_block": "4d6D9LJUZqo5Caq2qBDAvBaoRuQzMBrDzTk4zooTc2ua",
            "latest_protocol_version": 52,
            "next_bp_hash": "HQ7kLQBLEdPiSkgDNgEc48nu1FKMSp2GdJaL9E46JP7g",
            "next_epoch_id": "J3y2rw3GyXg1CeqjM9g8A551TfeS57eA7HuwFKT2h1ye",
            "outcome_root": "v8rmUoPJpof7UnDVdT6yjr9TRmDU8ETecXcg1UM2UFs",
            "prev_hash": "DvcFWAqdYUmNMMJ88HHFDYWd9X9yPo8dKf9xcTapgvgr",
            "prev_height": 86800608,
            "prev_state_root": "Amd8P2EZnFEkSqomotn3J8E92jwXizL36ENN5ZCFUSpG",
            "random_value": "G9PFKAuSNjkn1xNJb6hSnBR7Zi5DDsQSWwzEwAS57zDW",
            "rent_paid": "0",
            "signature": "ed25519:3H5CR4VTuys89BcNM6miFRgQXyn879wWzunygqb7TNhQmB2Pqu61AgJZDYSdZGYT45S3P9MDKhPzXuoQiu5VGCwi",
            "timestamp": 1649168106378663400,
            "timestamp_nanosec": "1649168106378663341",
            "total_supply": "2195153793571731315232923815317981",
            "validator_proposals": [],
            "validator_reward": "0"
        }
    }
}
```