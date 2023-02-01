---
description: Returns general status of a given node (sync status, nearcore node version, protocol version, etc), and the current set of validators.
---

# Node Status

### **Parameters**

- `method:` status
- `params:` []

### **Returns**

Returns general status of a given node (sync status, nearcore node version, protocol version, etc), and the current set of validators.

### **Example**

Request

```bash
curl https://rpc.<REGION>.gateway.fm/v4/near/non-archival/mainnet \
-X POST \
-H 'Content-Type: application/json' \
-H 'Authorization: Bearer <YOUR_API_KEY>' \
-d '{
  "jsonrpc": "2.0",
  "id": "11",
  "method": "status",
  "params": []
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "chain_id": "mainnet",
        "latest_protocol_version": 52,
        "protocol_version": 52,
        "rpc_addr": "0.0.0.0:3030",
        "sync_info": {
            "earliest_block_hash": "4bfmmYezWCiVxupQYw1ZqRzdJABU2Km83LBpQ4VrBV5V",
            "earliest_block_height": 62677761,
            "earliest_block_time": "2022-04-02T10:23:25.622541317Z",
            "latest_block_hash": "HBSTLn6iWGiUgG2bpEpt2Ctv9Niqc1LEe8DCxWcB3U8U",
            "latest_block_height": 62897763,
            "latest_block_time": "2022-04-05T16:13:05.221493608Z",
            "latest_state_root": "CKJp1Zp1SsPJy1ZvvN2kZeBVbP7Jq5cPuR5z3eGMybZ",
            "syncing": false
        },
        "validator_account_id": null,
        "validators": [
            {
                "account_id": "staked.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "astro-stakers.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "bzam6yjpnfnxsdmjf6pw.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "bisontrails.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "dragonfly.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "foundry.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "aurora.pool.near",
                "is_slashed": false
            },
            {
                "account_id": "finoa.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "epic.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "magic.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "electric.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "zavodil.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "rekt.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "d1.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "nearcrowd.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stake1.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "anonymous.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "blockdaemon.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "dokiacapital.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "08investinwomen_runbybisontrails.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "chorusone.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "binancenode1.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "accomplice.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "abl_pool.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "future_is_near.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "legends.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "hb436_pool.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "continue.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "openshards.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "figment.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "ideocolabventures.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "northernlights.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "buildlinks.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "nc2.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "smart-stake.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "pandora.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "nearfans.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "erm.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "nodeasy.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "cryptium.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stakin.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "lux.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "everstake.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "sharpdarts.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "hashquark.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "dsrvlabs.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "baziliknear.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "masternode24.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stakesabai.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "lunanova.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stardust.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "appload.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "republic.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "fish.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "jazza.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "moonlet.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "01node.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "inotel.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "fresh.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "zkv_staketosupportprivacy.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "staking_opp_disc.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "qbit.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "p2p-org.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "galaxydigital.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "lionstake.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "kosmos_and_p2p.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "prophet.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "vortex_live.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "centurion.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "sparkpool.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "binancestaking.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "dexagon.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "pathrocknetwork.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "ib.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "cryptogarik.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "infiniteloop.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "pandateam.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "optimusvalidatornetwork.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "cryptoblossom.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "ledgerbyfigment.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "incrypted.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "ni.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stakely_io.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "shardlabs.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "grassets.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "staking-power.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "bflame.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "inc4.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "doubletop.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "genesislab.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "sicmundus.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "4ire.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "lavenderfive.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "dariya.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "stakesstone.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "anchikovproduction.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "galactic.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "avado.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "steak.poolv1.near",
                "is_slashed": false
            },
            {
                "account_id": "near-fans.poolv1.near",
                "is_slashed": false
            }
        ],
        "version": {
            "build": "unknown",
            "version": "1.25.0"
        }
    }
}
```
