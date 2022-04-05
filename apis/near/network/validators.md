---
description: Queries active validators on the network returning details and the state of validation on the blockchain.
---

# Validation Status

### **Parameters**
* `method:` validators
* `params:`
  * `["block hash"]`, `[block number]`, or `[null]` for the latest block

### **Returns**
Queries active validators on the network returning details and the state of validation on the blockchain.

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
  "method": "validators",
  "params": [null]
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "current_fishermen": [],
        "current_proposals": [
            {
                "account_id": "01node.poolv1.near",
                "public_key": "ed25519:5xz7EbcnPqabwoFezdJBxieK8S7XLsdHHuLwM4vLLhFt",
                "stake": "1761870492857065922749163154624",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "08investinwomen_runbybisontrails.poolv1.near",
                "public_key": "ed25519:C6yqxQ3suwjmm8ufG5e3BsHiwxUs9h839FCneF41V7TM",
                "stake": "5528385303504862712858001320797",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "4ire.poolv1.near",
                "public_key": "ed25519:GdirfFSuT3t1ChEMqwcV6zko5Ya9yVAqm6Pnhk9qcXvS",
                "stake": "178680614749632691278924738838",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "abl_pool.poolv1.near",
                "public_key": "ed25519:5nnwJr7WgMXbWiudFcen9AMXRUXWA3ij6GGFZvRWXA3C",
                "stake": "5235606465327759598998584721942",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "accomplice.poolv1.near",
                "public_key": "ed25519:5ck255MtkoGQxh9LfjNtdb4M7WHkUmjU7SBJCEkZP2B7",
                "stake": "5257123206757017184120900800745",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "anchikovproduction.poolv1.near",
                "public_key": "ed25519:HMhR7VGBwC4GDyDpDRrgdArvCXmjhEvgu2X7iiCnikTJ",
                "stake": "184150666291775360543324537944",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "anonymous.poolv1.near",
                "public_key": "ed25519:Hoj7LbPwNwAkLFhf8z2aDF1BG6NDSrq1BfkdaKqPfbXx",
                "stake": "6258409764778892538122339541787",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "appload.poolv1.near",
                "public_key": "ed25519:6LbMVL6otkvZbpuC9sN3z7EXSMo3PT9noPeBdBZTFneM",
                "stake": "2544894127169171685346077741661",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "astro-stakers.poolv1.near",
                "public_key": "ed25519:2nPSBCzjqikgwrqUMcuEVReJhmkC91eqJGPGqH9sZc28",
                "stake": "24275305805207952813826233944237",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "aurora.pool.near",
                "public_key": "ed25519:FZKXoWHFCXMrKiXjAKFdHo5g9PDom4bWMRFERBfufi2Y",
                "stake": "17829799583899358498779695671327",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "avado.poolv1.near",
                "public_key": "ed25519:FdLWsf42e3Sc7bdKMtxJMgWRP21ysZDSXFnS2vTwTaaA",
                "stake": "115683815475432969686500782890",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "baziliknear.poolv1.near",
                "public_key": "ed25519:E4LAWdgLifBEoaWvhRNy5vpdAnUc3GsUHePeiAurZY5v",
                "stake": "2993264704626453687870873718693",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "bflame.poolv1.near",
                "public_key": "ed25519:6QDZab171amvZ8ZP3k2UqiwqcYBBD3HjC3ErYJ7ndWCK",
                "stake": "188007636178271819594832011362",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "binancenode1.poolv1.near",
                "public_key": "ed25519:Bb7uPEocbsiQwRfPmsiiiM88DodtuYnBDi6dKZ4JZo2N",
                "stake": "5335324156602714583268755923321",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "binancestaking.poolv1.near",
                "public_key": "ed25519:H9o1RgTXZjBwD5GUEajbHy6S7UoeNYMwsqueCeadkHPH",
                "stake": "279776115079388805638035520293",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "bisontrails.poolv1.near",
                "public_key": "ed25519:Emk6wQJtpQZRJCvvPmmwP9GD2Pk37xxRpmb5uRvJpX62",
                "stake": "20640352588650366551368343092867",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "blockdaemon.poolv1.near",
                "public_key": "ed25519:3GNFSJiFQQ1rnR68T4eZRff2omPhg1CTewUHBJpQAdyc",
                "stake": "6819284656626167848268254721858",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "buildlinks.poolv1.near",
                "public_key": "ed25519:Hd3irGt4zEqRPAzcFszX3oTkVWRFFxdecDvShCJSS1Wg",
                "stake": "4143098666161084262359171808129",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "bzam6yjpnfnxsdmjf6pw.poolv1.near",
                "public_key": "ed25519:2ZJqaaCAisK4u8E2i611zFfvNmrvevovnU3M7SpGHkLY",
                "stake": "23585103803285922693679099195074",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "centurion.poolv1.near",
                "public_key": "ed25519:66eogeJGkWhoipU3YE3QapJbvYRXze6rg4BE6g7kDBRk",
                "stake": "410118582494497236179803941404",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "chelovek_iz_naroda.poolv1.near",
                "public_key": "ed25519:3dNkgMq1rksoS3XuhmZaX35iqaerXbLHyytRQ5Dfj3Rt",
                "stake": "103442332716527806784054165087",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "chorusone.poolv1.near",
                "public_key": "ed25519:AZwJAgu2qRxHwdpj8ioZEFGcc2jbaZGN7ZvUe7CuXtM7",
                "stake": "5468852408985414127449280115061",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "continue.poolv1.near",
                "public_key": "ed25519:9rDZywYL3tnvzj6hnePw3MaPFPfSeSCLxBp1niTGbMaK",
                "stake": "4756491051927287689548093112582",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "cryptium.poolv1.near",
                "public_key": "ed25519:5Y9hW8cKBb5RnsJBqttHHC5ujz5zcZZ5xnrJPwkCWmGQ",
                "stake": "3500808051408852143386453212996",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "cryptoblossom.poolv1.near",
                "public_key": "ed25519:5opTNJEkCBYuyMgAghY2Sxp4bBtXYQtbEvZ3Wc5Awohb",
                "stake": "250878497082688208905115238797",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "cryptogarik.poolv1.near",
                "public_key": "ed25519:45zFAC8pLgwn1d5pSBpBHesWbzngfRgd92zaom7K8m8j",
                "stake": "276692264998374310607401692472",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "cryptotribe.poolv1.near",
                "public_key": "ed25519:Hi4Avivjo4DKFbNN9Q4Z7QSxEjkix9NEM27raEvDr22j",
                "stake": "39480853912728527990012670303",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "d1.poolv1.near",
                "public_key": "ed25519:7ZhMRwnSHGJtWjGBZiRhhSi6XyqKeNHtnEXsVTNdrsk6",
                "stake": "7233513292930414256517760258828",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "dariya.poolv1.near",
                "public_key": "ed25519:AJc9P74HBXGas6mqpA8XJDWgNzM9ZLxYiH6q7cdY75pn",
                "stake": "176665902929790471105496826857",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "dexagon.poolv1.near",
                "public_key": "ed25519:AQHwptR3Ho348BpFXJDjkxpWMW5ZwN7xWM3XWAWSEEgs",
                "stake": "291341209349107570289834158563",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "dokiacapital.poolv1.near",
                "public_key": "ed25519:FGcJJeWMyx1xDbfkcPM2oMeUeGaADJuPmeqx5rjsHn7t",
                "stake": "5898608673256871316861706443345",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "doubletop.poolv1.near",
                "public_key": "ed25519:G5YQUqsVJd1qR2N7tQsxuZGW6izE6Kx8i2F5fDVKUJ39",
                "stake": "194564718650362542467526196891",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "dragonfly.poolv1.near",
                "public_key": "ed25519:6Gj8MRp9KqfdiXa35LJcZnqeBNNEZoYk6ysvpzHaruvq",
                "stake": "19851064799061486999806955517222",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "dsrvlabs.poolv1.near",
                "public_key": "ed25519:9SACdsDDgXA2WZLfJvpkKbu22Exxtc4CMbeHmVnN2P4a",
                "stake": "3076761509568605855613581029293",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "electric.poolv1.near",
                "public_key": "ed25519:GpSr5KAZMZ1Cb4dHMRUVhmp95y2fmWtm4dEjAr8iAva5",
                "stake": "9757452720768981090129444342863",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "epic.poolv1.near",
                "public_key": "ed25519:68HExKDtw1CjGzopZ8fMAMhMSZRVKRhwLzLQmGKtFNzT",
                "stake": "11541823189745839335733862535550",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "erm.poolv1.near",
                "public_key": "ed25519:88nnN6LAuCbJaj9wucd1WUMfTtdv2s3njpvozHft8oQ5",
                "stake": "3579477620604453826328033368972",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "everstake.poolv1.near",
                "public_key": "ed25519:4JLvwa1r2eAxHLyKeDJnpqMG5f2Z9rr49rwuTwb9g8u2",
                "stake": "3338763858056929590559589843836",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "figment.poolv1.near",
                "public_key": "ed25519:7RjyY1bRKDqkshbKZtgpQdwsdxou8j9my8g1hPKZ9ngM",
                "stake": "4479744165026377810289963243636",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "finoa.poolv1.near",
                "public_key": "ed25519:62gxgzoie7FiK9dnWuiwM1bbuvhpceYDavK7SgdfEMJc",
                "stake": "14114760670406389384847147854510",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "fish.poolv1.near",
                "public_key": "ed25519:27KegJd17HeXHk9h5MqkT35QAuvYvo5GFgPTpSVU4kPN",
                "stake": "2195986354656240355377453562270",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "foundry.poolv1.near",
                "public_key": "ed25519:5Qx8Fq3SK4Vu1sRRpf2HsNGLAqdNqgkKEebHMniLWhkW",
                "stake": "19198992750840729648115183170052",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "fresh.poolv1.near",
                "public_key": "ed25519:6YHLXhohY8kMnkp5Jw4HrJ52xtdyt1rcP6AaWkKzh3ED",
                "stake": "1202693963745632067554600802698",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "future_is_near.poolv1.near",
                "public_key": "ed25519:F3vEGwYYGisaXwKJWrYgorB95DfArDby8bK5wydxD5fp",
                "stake": "5161502904606375159244477856621",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "galactic.poolv1.near",
                "public_key": "ed25519:GFK83N32DbERtFg8rkpfNBsKtkFpmNQzyKFM9kJvPCMG",
                "stake": "173491240517369601706825283846",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "galaxydigital.poolv1.near",
                "public_key": "ed25519:8ZD8CcSzSfVsYo7XyABHJsYcrpBE3EL5MwukoEfrNYMR",
                "stake": "522882646303315705924331753454",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "genesislab.poolv1.near",
                "public_key": "ed25519:Do8QywDQ9DBvHaoxSwzAhuejv3ZU8CFkQ9xWWnHVaQRM",
                "stake": "179965764566198288943851204172",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "grassets.poolv1.near",
                "public_key": "ed25519:GS8uhr7mhsBWB5c1JgvsJzpwZDGrcnB9Xnw7YRyMSQP5",
                "stake": "191923102199267052111461392277",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "guli.poolv1.near",
                "public_key": "ed25519:14hEUZxmfTrame1J9HqnnRYdDDKAJjNH1ZcfnBPrUMJN",
                "stake": "100999880872622539213930891867",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "hashquark.poolv1.near",
                "public_key": "ed25519:3YDdmN1vhF7yAWnYxGMHY46jcLE9h11HvEeF6Kntugeq",
                "stake": "3049913044424343375894391988823",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "hb436_pool.poolv1.near",
                "public_key": "ed25519:7oU4C3vWqkeup7aMfjyV1ojt7yKX7ShLfvNCahBRy1eW",
                "stake": "4907444704548434462248641022770",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "ib.poolv1.near",
                "public_key": "ed25519:8jeZyfvtTDGNyLVwLKEiCQZrq6J8hHLcV6bsDKZQ4iia",
                "stake": "282741769305884182576241368281",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "ideocolabventures.poolv1.near",
                "public_key": "ed25519:6NFuvrmnJiokXibR9Z7TUHjB4NJnD1rJAHhBu9JWmBdh",
                "stake": "4461246909758661071745035680284",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "inc4.poolv1.near",
                "public_key": "ed25519:EPK4Cnkuua9vH75Rq5f6r66fcfR6eFi5pS3o5iiV7hKP",
                "stake": "194497887280362709450007978298",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "incrypted.poolv1.near",
                "public_key": "ed25519:CsnkDDxNP6ukieSgz31dz9rA3UDKamKB2So2iABVhubi",
                "stake": "212877046075336031249512885924",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "infiniteloop.poolv1.near",
                "public_key": "ed25519:9BUwtDegzwKcmJBjLgUDLHc3pePgPKcWJXYGcZb33Nyr",
                "stake": "271920270597133429401217626662",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "infstones.poolv1.near",
                "public_key": "ed25519:23LabqKAAcBfAoJcNmMVWWHAnGkRjWo8VPH34wHi4tiG",
                "stake": "100031014441559896798544173998",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "inotel.poolv1.near",
                "public_key": "ed25519:DmEDRntb9NwfbfdvDf6wzjsw1vxzQcJAAhFL2J75iLwr",
                "stake": "1689266911242107725696272936356",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "jazza.poolv1.near",
                "public_key": "ed25519:EW66Fkv7XcE9FiybuYtVURjHhYeEgwWWpzF685Vi7foY",
                "stake": "1880584406558872152939249745285",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "kosmos_and_p2p.poolv1.near",
                "public_key": "ed25519:41GWxdQHe4Y2fuisvz5k5G2NwDFEavRkisoZkB5tfJuC",
                "stake": "449820531398296018040555722725",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "lavenderfive.poolv1.near",
                "public_key": "ed25519:HXiLVGFiMssLHH6H36G7AsaYhBankPNgd4b7uNsXzQVF",
                "stake": "186399293635238607142333611364",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "ledgerbyfigment.poolv1.near",
                "public_key": "ed25519:4JJTNeMaSb8W3NELh2rkkrDCqG1VpM3gdJ1hc9HFTBmN",
                "stake": "214838178699292744407764285775",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "legends.poolv1.near",
                "public_key": "ed25519:DNK46DeHKeJPF9YetmNxZnqtpkeLjdUb9ezSRCue3TpB",
                "stake": "5022407164364458975465220351563",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "lionstake.poolv1.near",
                "public_key": "ed25519:8kciZQy815tZooy7HPJkBq2cyEw9L7fbsWcmWLgwG4m3",
                "stake": "509009701344340115680769752716",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "lunanova.poolv1.near",
                "public_key": "ed25519:qkfP4NsSuHybdLhdvvYQ2Y9xWPsd249thEvrzbJBKNc",
                "stake": "2631192954398150307368082212447",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "lux.poolv1.near",
                "public_key": "ed25519:HzTGTDfTz63QGvvUdMGozFeaENFGyYAoSrqYJb23qZFN",
                "stake": "3338884542125774016247972347266",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "magic.poolv1.near",
                "public_key": "ed25519:5fwufMXx9CTyLRkz7x3htQa3rFGzFZuz6d43LhCTmKCS",
                "stake": "10521641593284981281370191134122",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "masternode24.poolv1.near",
                "public_key": "ed25519:5ZyaXsGCya4Sch5bqUfohvo7iRFYB9ancRouggWRsiDU",
                "stake": "2930871683367270577889033641226",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "moonlet.poolv1.near",
                "public_key": "ed25519:GkDwzPckMfhkdYgyFG69Uph8RJ12BcV9xNeZW2q93ZJD",
                "stake": "1815826157246859155895550891314",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "n0ok.poolv1.near",
                "public_key": "ed25519:EC1p3w9hd4XkYoUiAKc8PSQGVFGiUXTDJvqkurRdAFz5",
                "stake": "103705468202690873505067169183",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "nc2.poolv1.near",
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "stake": "4129184007203271991290104361177",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "near-fans.poolv1.near",
                "public_key": "ed25519:AgV97ssnHm7qN8JhYZjwyDtuaT6Ms3Fgbw3WeAC8M3iF",
                "stake": "119993055537196689525376544490",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "nearcrowd.poolv1.near",
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "stake": "7068212732142351651911202216043",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "nearfans.poolv1.near",
                "public_key": "ed25519:GM8vWM4TqTt7jh3sXYCAs2KPyn4vEmAceteBGEFYhyku",
                "stake": "3611678565984013999515923042976",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "ni.poolv1.near",
                "public_key": "ed25519:8sRAjT6nFnCtGmppKXFuwqvRre5EPspZCLncFc5Aok7z",
                "stake": "207662013252305042583575548513",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "nodeasy.poolv1.near",
                "public_key": "ed25519:8mjespqqUePSYSsxYxPqCUsZUuMxVJr1vjBRwFeCke5K",
                "stake": "3551855057278610581928904575021",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "northernlights.poolv1.near",
                "public_key": "ed25519:7HXh6iS9Rh92Uj1c5T9fPjQXPLnti4Rr2cJQcJEYpdGV",
                "stake": "4336664106666710408564022080785",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "openshards.poolv1.near",
                "public_key": "ed25519:4Xm73PiAGMZu3mZg4gF7j96iTAFHGbPvqzxBaTgKP4ub",
                "stake": "4507194826435451735192953451648",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "optimusvalidatornetwork.poolv1.near",
                "public_key": "ed25519:C3CJMKaWdEzkqyNCKwnKud6wDNnzs7Ura63k16zm4LUU",
                "stake": "258272543497050490106761200209",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "p2p-org.poolv1.near",
                "public_key": "ed25519:J441YAvvYvjWs3aVzjc5KLLWRzmhQTEMaymPyWFkMGeG",
                "stake": "550902301335499162054892926093",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "pandateam.poolv1.near",
                "public_key": "ed25519:Cu83NRziNLiT6HLu9kJ8svFoftZQ9wVmjScxjqCybppt",
                "stake": "258527911188231311194898260976",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "pandora.poolv1.near",
                "public_key": "ed25519:53N7KBhSkEP6tLuQmxZV9fAK16D1C2kWnuzes8KNyS7P",
                "stake": "3793981582239176298150043570298",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "pathrocknetwork.poolv1.near",
                "public_key": "ed25519:2iJQLVXubWafG7K1NzGVvjP54UJCgVg3cuPMktw8r7uQ",
                "stake": "285829517627947960019566663893",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "projecttent.poolv1.near",
                "public_key": "ed25519:9qtkAbFDuAuEDLaGkAV5MHmFSKEtczuxDWYc2eKgXCx8",
                "stake": "106241869869295567899124264258",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "prophet.poolv1.near",
                "public_key": "ed25519:BV5b4DpgCUy1TEitE4TVPhpTY7uDNpHc8DBPyH6cYCBq",
                "stake": "425275115683540172140846353189",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "qbit.poolv1.near",
                "public_key": "ed25519:5DqZLnDu6PMEyhJzc5NhiMsoWeYMWG1bC4AULyafoXMv",
                "stake": "616847597262546504868216266304",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "rekt.poolv1.near",
                "public_key": "ed25519:FoAaUdVKEHtVokG1aVmJNou61YcfQhXmaZ5Hnfsz4fHC",
                "stake": "9417189526172407052697779058141",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "republic.poolv1.near",
                "public_key": "ed25519:5sT6xtwxvLARW6y3KURYmyFd5SokJFhiK4jyqbamzzZ6",
                "stake": "2483064257751378740248020594647",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "shardlabs.poolv1.near",
                "public_key": "ed25519:Gj5ToPBT4Ygh6CFT654bf1Y2FkWQAA7KFNCkeRGEV4VB",
                "stake": "193413786576949280986243246409",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "sharpdarts.poolv1.near",
                "public_key": "ed25519:9XMHXqv7rM3QQxzjUu7dfKD7GhMkq8CEceaPdkhiBQUX",
                "stake": "3237310305189066724157090848752",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "sicmundus.poolv1.near",
                "public_key": "ed25519:Fh4pUKGsCVqutYHS52RLCA7UpLaCVWF5LZ9xXo94zQBw",
                "stake": "187053325592174059462851875228",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "smart-stake.poolv1.near",
                "public_key": "ed25519:A6wpkLQiYqPZ1rbd9s5S1Bg3LxccVsQqiCRDUXwzJ6Hx",
                "stake": "3897557588749438905867636134110",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "sparkpool.poolv1.near",
                "public_key": "ed25519:4GdDoLduepfbMCD9M3UUQ1jedRHv4cWWn6VEkoax8dT2",
                "stake": "344428295623315269991176278017",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stake1.poolv1.near",
                "public_key": "ed25519:7EiVt9i7SmULDKEnAXBFSMzwUmZdxUYDFkP73MZuCH1h",
                "stake": "9361413227896895218543477045689",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "staked.poolv1.near",
                "public_key": "ed25519:3JBVXqenru2ErAM1kHQ8qfd29dCkURLd6JKrFgtmcDTZ",
                "stake": "43368186895152622308282792177769",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stakely_io.poolv1.near",
                "public_key": "ed25519:HWp9E3gP91s25ddMS9xUWuzbJUpVGiPoitu5bT6hqMHs",
                "stake": "208005147836654022188993034607",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stakesabai.poolv1.near",
                "public_key": "ed25519:6abauNvvWnEkagjVpWRy2tZJdzPkmqurUjteMTKk5KQF",
                "stake": "2931736620123102109198891387364",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stakesstone.poolv1.near",
                "public_key": "ed25519:crXSnXFFbBr3eCXPeV54bUPm6m4D4EYgLzUmxM2G9FU",
                "stake": "187336394311416747048145276914",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stakin.poolv1.near",
                "public_key": "ed25519:85UGfKdVoxX9u86JsBMxmVHBguYonnM3vTR2WoD5GkEg",
                "stake": "3784427598224175275512246181115",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "staking-power.poolv1.near",
                "public_key": "ed25519:42ikqyV1BYmSnhHJ9EsLLy9kgeAg1mC3qqU1AJGaTEaW",
                "stake": "189650718938551026943410322845",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "staking_opp_disc.poolv1.near",
                "public_key": "ed25519:8XbCfLQVSwtwaBajvByG87CxPPbaFdryz5qEkde1fSGv",
                "stake": "944721055959917522878780258076",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "stardust.poolv1.near",
                "public_key": "ed25519:6rxCJpTnrT6NFuGg6d5Dj3FEUz1ScNU9u35ywB3dYhrX",
                "stake": "2566198485642516835969917673017",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "steak.poolv1.near",
                "public_key": "ed25519:3tZG4QgzWpTKt2dChqZVUTBvF35pvG7BHyyJULF8VXQc",
                "stake": "111810432652471278058698847828",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "vortex_live.poolv1.near",
                "public_key": "ed25519:GrPW17VhMVLi15JohsM2ag2GpcqpQuJNm3Hf6vPYXRYZ",
                "stake": "414319874441706538463794487896",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "zavodil.poolv1.near",
                "public_key": "ed25519:HHARoU1hANWF9hu7YRstDDvgyigBhUeUuqecRVr8dpUz",
                "stake": "9900748939557022776365916590873",
                "validator_stake_struct_version": "V1"
            },
            {
                "account_id": "zkv_staketosupportprivacy.poolv1.near",
                "public_key": "ed25519:2kAo86DW8mDaLDg37rFhQY8UYSZVq1CtegUHBEDvpSMA",
                "stake": "1148062516430984640092325514593",
                "validator_stake_struct_version": "V1"
            }
        ],
        "current_validators": [
            {
                "account_id": "staked.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 2878,
                "num_expected_chunks": 11512,
                "num_produced_blocks": 2878,
                "num_produced_chunks": 11512,
                "public_key": "ed25519:3JBVXqenru2ErAM1kHQ8qfd29dCkURLd6JKrFgtmcDTZ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "43361709520716817718356196764387"
            },
            {
                "account_id": "astro-stakers.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 1619,
                "num_expected_chunks": 6476,
                "num_produced_blocks": 1619,
                "num_produced_chunks": 6476,
                "public_key": "ed25519:2nPSBCzjqikgwrqUMcuEVReJhmkC91eqJGPGqH9sZc28",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "24257181698082537421521507049706"
            },
            {
                "account_id": "bzam6yjpnfnxsdmjf6pw.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 1523,
                "num_expected_chunks": 6092,
                "num_produced_blocks": 1523,
                "num_produced_chunks": 6092,
                "public_key": "ed25519:2ZJqaaCAisK4u8E2i611zFfvNmrvevovnU3M7SpGHkLY",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "23580549125295224292864424559083"
            },
            {
                "account_id": "bisontrails.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 1303,
                "num_expected_chunks": 5212,
                "num_produced_blocks": 1303,
                "num_produced_chunks": 5212,
                "public_key": "ed25519:Emk6wQJtpQZRJCvvPmmwP9GD2Pk37xxRpmb5uRvJpX62",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "20637963375456936627562228125373"
            },
            {
                "account_id": "dragonfly.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 1291,
                "num_expected_chunks": 5164,
                "num_produced_blocks": 1291,
                "num_produced_chunks": 5164,
                "public_key": "ed25519:6Gj8MRp9KqfdiXa35LJcZnqeBNNEZoYk6ysvpzHaruvq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "19847210256638200748554896603965"
            },
            {
                "account_id": "foundry.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 1264,
                "num_expected_chunks": 5056,
                "num_produced_blocks": 1264,
                "num_produced_chunks": 5056,
                "public_key": "ed25519:5Qx8Fq3SK4Vu1sRRpf2HsNGLAqdNqgkKEebHMniLWhkW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "19195219017787289470533402206624"
            },
            {
                "account_id": "aurora.pool.near",
                "is_slashed": false,
                "num_expected_blocks": 1158,
                "num_expected_chunks": 4632,
                "num_produced_blocks": 1158,
                "num_produced_chunks": 4632,
                "public_key": "ed25519:FZKXoWHFCXMrKiXjAKFdHo5g9PDom4bWMRFERBfufi2Y",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "16962158509492671875939893197670"
            },
            {
                "account_id": "finoa.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 991,
                "num_expected_chunks": 3964,
                "num_produced_blocks": 991,
                "num_produced_chunks": 3964,
                "public_key": "ed25519:62gxgzoie7FiK9dnWuiwM1bbuvhpceYDavK7SgdfEMJc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "14113538017156548848358414940085"
            },
            {
                "account_id": "epic.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 768,
                "num_expected_chunks": 3072,
                "num_produced_blocks": 768,
                "num_produced_chunks": 3072,
                "public_key": "ed25519:68HExKDtw1CjGzopZ8fMAMhMSZRVKRhwLzLQmGKtFNzT",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "11525805616201107991689973544079"
            },
            {
                "account_id": "magic.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 719,
                "num_expected_chunks": 2876,
                "num_produced_blocks": 719,
                "num_produced_chunks": 2876,
                "public_key": "ed25519:5fwufMXx9CTyLRkz7x3htQa3rFGzFZuz6d43LhCTmKCS",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "10603010712136762851333777383822"
            },
            {
                "account_id": "electric.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 666,
                "num_expected_chunks": 2660,
                "num_produced_blocks": 666,
                "num_produced_chunks": 2660,
                "public_key": "ed25519:GpSr5KAZMZ1Cb4dHMRUVhmp95y2fmWtm4dEjAr8iAva5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9755568293879982627064875724292"
            },
            {
                "account_id": "zavodil.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 613,
                "num_expected_chunks": 2452,
                "num_produced_blocks": 613,
                "num_produced_chunks": 2452,
                "public_key": "ed25519:HHARoU1hANWF9hu7YRstDDvgyigBhUeUuqecRVr8dpUz",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9487509922201578045079499376539"
            },
            {
                "account_id": "rekt.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 610,
                "num_expected_chunks": 2440,
                "num_produced_blocks": 610,
                "num_produced_chunks": 2440,
                "public_key": "ed25519:FoAaUdVKEHtVokG1aVmJNou61YcfQhXmaZ5Hnfsz4fHC",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9400907860074135521636112337807"
            },
            {
                "account_id": "d1.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 503,
                "num_expected_chunks": 2012,
                "num_produced_blocks": 503,
                "num_produced_chunks": 2012,
                "public_key": "ed25519:7ZhMRwnSHGJtWjGBZiRhhSi6XyqKeNHtnEXsVTNdrsk6",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "7267307541545428175704260002602"
            },
            {
                "account_id": "nearcrowd.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 432,
                "num_expected_chunks": 1728,
                "num_produced_blocks": 432,
                "num_produced_chunks": 1728,
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "7066847655273024827991072246516"
            },
            {
                "account_id": "stake1.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 438,
                "num_expected_chunks": 1752,
                "num_produced_blocks": 438,
                "num_produced_chunks": 1752,
                "public_key": "ed25519:7EiVt9i7SmULDKEnAXBFSMzwUmZdxUYDFkP73MZuCH1h",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "6449036077120685626829777045689"
            },
            {
                "account_id": "anonymous.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 419,
                "num_expected_chunks": 1676,
                "num_produced_blocks": 419,
                "num_produced_chunks": 1676,
                "public_key": "ed25519:Hoj7LbPwNwAkLFhf8z2aDF1BG6NDSrq1BfkdaKqPfbXx",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "6257201160818753897136952926507"
            },
            {
                "account_id": "blockdaemon.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 377,
                "num_expected_chunks": 1508,
                "num_produced_blocks": 377,
                "num_produced_chunks": 1508,
                "public_key": "ed25519:3GNFSJiFQQ1rnR68T4eZRff2omPhg1CTewUHBJpQAdyc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5966673972483511717610669328593"
            },
            {
                "account_id": "dokiacapital.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 400,
                "num_expected_chunks": 1600,
                "num_produced_blocks": 400,
                "num_produced_chunks": 1600,
                "public_key": "ed25519:FGcJJeWMyx1xDbfkcPM2oMeUeGaADJuPmeqx5rjsHn7t",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5897335935910727649351633375784"
            },
            {
                "account_id": "08investinwomen_runbybisontrails.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 376,
                "num_expected_chunks": 1504,
                "num_produced_blocks": 376,
                "num_produced_chunks": 1504,
                "public_key": "ed25519:C6yqxQ3suwjmm8ufG5e3BsHiwxUs9h839FCneF41V7TM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5527319306589094597067054972054"
            },
            {
                "account_id": "chorusone.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 377,
                "num_expected_chunks": 1508,
                "num_produced_blocks": 377,
                "num_produced_chunks": 1508,
                "public_key": "ed25519:AZwJAgu2qRxHwdpj8ioZEFGcc2jbaZGN7ZvUe7CuXtM7",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5468402311820593854067510991822"
            },
            {
                "account_id": "binancenode1.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 371,
                "num_expected_chunks": 1484,
                "num_produced_blocks": 371,
                "num_produced_chunks": 1484,
                "public_key": "ed25519:Bb7uPEocbsiQwRfPmsiiiM88DodtuYnBDi6dKZ4JZo2N",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5333927553303890175106954845405"
            },
            {
                "account_id": "accomplice.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 338,
                "num_expected_chunks": 1352,
                "num_produced_blocks": 338,
                "num_produced_chunks": 1352,
                "public_key": "ed25519:5ck255MtkoGQxh9LfjNtdb4M7WHkUmjU7SBJCEkZP2B7",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5256115564953589373755901945310"
            },
            {
                "account_id": "abl_pool.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 337,
                "num_expected_chunks": 1348,
                "num_produced_blocks": 337,
                "num_produced_chunks": 1348,
                "public_key": "ed25519:5nnwJr7WgMXbWiudFcen9AMXRUXWA3ij6GGFZvRWXA3C",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5234595381849866992680522712615"
            },
            {
                "account_id": "future_is_near.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 351,
                "num_expected_chunks": 1404,
                "num_produced_blocks": 351,
                "num_produced_chunks": 1404,
                "public_key": "ed25519:F3vEGwYYGisaXwKJWrYgorB95DfArDby8bK5wydxD5fp",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5149364142019401325877737746001"
            },
            {
                "account_id": "legends.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 314,
                "num_expected_chunks": 1256,
                "num_produced_blocks": 314,
                "num_produced_chunks": 1256,
                "public_key": "ed25519:DNK46DeHKeJPF9YetmNxZnqtpkeLjdUb9ezSRCue3TpB",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5020478464500699127972362974740"
            },
            {
                "account_id": "hb436_pool.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 311,
                "num_expected_chunks": 1244,
                "num_produced_blocks": 311,
                "num_produced_chunks": 1244,
                "public_key": "ed25519:7oU4C3vWqkeup7aMfjyV1ojt7yKX7ShLfvNCahBRy1eW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4906496994492782566364827474124"
            },
            {
                "account_id": "continue.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 349,
                "num_expected_chunks": 1396,
                "num_produced_blocks": 349,
                "num_produced_chunks": 1396,
                "public_key": "ed25519:9rDZywYL3tnvzj6hnePw3MaPFPfSeSCLxBp1niTGbMaK",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4742932097534735914526608229923"
            },
            {
                "account_id": "openshards.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 299,
                "num_expected_chunks": 1196,
                "num_produced_blocks": 299,
                "num_produced_chunks": 1196,
                "public_key": "ed25519:4Xm73PiAGMZu3mZg4gF7j96iTAFHGbPvqzxBaTgKP4ub",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4516693351678229225775346215390"
            },
            {
                "account_id": "figment.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 309,
                "num_expected_chunks": 1236,
                "num_produced_blocks": 309,
                "num_produced_chunks": 1236,
                "public_key": "ed25519:7RjyY1bRKDqkshbKZtgpQdwsdxou8j9my8g1hPKZ9ngM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4478898954915445284049642835381"
            },
            {
                "account_id": "ideocolabventures.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 319,
                "num_expected_chunks": 1276,
                "num_produced_blocks": 319,
                "num_produced_chunks": 1276,
                "public_key": "ed25519:6NFuvrmnJiokXibR9Z7TUHjB4NJnD1rJAHhBu9JWmBdh",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4460375475210333465458110811368"
            },
            {
                "account_id": "northernlights.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 277,
                "num_expected_chunks": 1108,
                "num_produced_blocks": 277,
                "num_produced_chunks": 1108,
                "public_key": "ed25519:7HXh6iS9Rh92Uj1c5T9fPjQXPLnti4Rr2cJQcJEYpdGV",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4355822761455102745180757912473"
            },
            {
                "account_id": "buildlinks.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 260,
                "num_expected_chunks": 1040,
                "num_produced_blocks": 260,
                "num_produced_chunks": 1040,
                "public_key": "ed25519:Hd3irGt4zEqRPAzcFszX3oTkVWRFFxdecDvShCJSS1Wg",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4142358369234478085631418750193"
            },
            {
                "account_id": "nc2.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 260,
                "num_expected_chunks": 1040,
                "num_produced_blocks": 260,
                "num_produced_chunks": 1040,
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4128362451010565455377742876485"
            },
            {
                "account_id": "smart-stake.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 252,
                "num_expected_chunks": 1008,
                "num_produced_blocks": 252,
                "num_produced_chunks": 1008,
                "public_key": "ed25519:A6wpkLQiYqPZ1rbd9s5S1Bg3LxccVsQqiCRDUXwzJ6Hx",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3881613985000877094427764083926"
            },
            {
                "account_id": "pandora.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 248,
                "num_expected_chunks": 992,
                "num_produced_blocks": 248,
                "num_produced_chunks": 992,
                "public_key": "ed25519:53N7KBhSkEP6tLuQmxZV9fAK16D1C2kWnuzes8KNyS7P",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3793146822011040042783462450708"
            },
            {
                "account_id": "nearfans.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 221,
                "num_expected_chunks": 884,
                "num_produced_blocks": 221,
                "num_produced_chunks": 884,
                "public_key": "ed25519:GM8vWM4TqTt7jh3sXYCAs2KPyn4vEmAceteBGEFYhyku",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3611382515803909118838809281885"
            },
            {
                "account_id": "erm.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 237,
                "num_expected_chunks": 948,
                "num_produced_blocks": 237,
                "num_produced_chunks": 948,
                "public_key": "ed25519:88nnN6LAuCbJaj9wucd1WUMfTtdv2s3njpvozHft8oQ5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3578918259582796043694837075049"
            },
            {
                "account_id": "nodeasy.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 260,
                "num_expected_chunks": 1040,
                "num_produced_blocks": 260,
                "num_produced_chunks": 1040,
                "public_key": "ed25519:8mjespqqUePSYSsxYxPqCUsZUuMxVJr1vjBRwFeCke5K",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3541483736223368643877805737164"
            },
            {
                "account_id": "cryptium.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 234,
                "num_expected_chunks": 936,
                "num_produced_blocks": 234,
                "num_produced_chunks": 936,
                "public_key": "ed25519:5Y9hW8cKBb5RnsJBqttHHC5ujz5zcZZ5xnrJPwkCWmGQ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3523963989399858515188950100807"
            },
            {
                "account_id": "stakin.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 270,
                "num_expected_chunks": 1080,
                "num_produced_blocks": 270,
                "num_produced_chunks": 1080,
                "public_key": "ed25519:85UGfKdVoxX9u86JsBMxmVHBguYonnM3vTR2WoD5GkEg",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3522399856856869612957604412626"
            },
            {
                "account_id": "lux.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 251,
                "num_expected_chunks": 1004,
                "num_produced_blocks": 251,
                "num_produced_chunks": 1004,
                "public_key": "ed25519:HzTGTDfTz63QGvvUdMGozFeaENFGyYAoSrqYJb23qZFN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3338107293242776952136941708693"
            },
            {
                "account_id": "everstake.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 237,
                "num_expected_chunks": 948,
                "num_produced_blocks": 237,
                "num_produced_chunks": 948,
                "public_key": "ed25519:4JLvwa1r2eAxHLyKeDJnpqMG5f2Z9rr49rwuTwb9g8u2",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3327596162892729739304036465863"
            },
            {
                "account_id": "sharpdarts.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 215,
                "num_expected_chunks": 860,
                "num_produced_blocks": 215,
                "num_produced_chunks": 860,
                "public_key": "ed25519:9XMHXqv7rM3QQxzjUu7dfKD7GhMkq8CEceaPdkhiBQUX",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3238952262878716930949128323884"
            },
            {
                "account_id": "hashquark.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 187,
                "num_expected_chunks": 748,
                "num_produced_blocks": 186,
                "num_produced_chunks": 744,
                "public_key": "ed25519:3YDdmN1vhF7yAWnYxGMHY46jcLE9h11HvEeF6Kntugeq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3119939510176430628461684012508"
            },
            {
                "account_id": "dsrvlabs.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 206,
                "num_expected_chunks": 824,
                "num_produced_blocks": 206,
                "num_produced_chunks": 824,
                "public_key": "ed25519:9SACdsDDgXA2WZLfJvpkKbu22Exxtc4CMbeHmVnN2P4a",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3076167336831410161078048650406"
            },
            {
                "account_id": "baziliknear.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 196,
                "num_expected_chunks": 784,
                "num_produced_blocks": 196,
                "num_produced_chunks": 784,
                "public_key": "ed25519:E4LAWdgLifBEoaWvhRNy5vpdAnUc3GsUHePeiAurZY5v",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2981949325794111271415952586290"
            },
            {
                "account_id": "masternode24.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 196,
                "num_expected_chunks": 784,
                "num_produced_blocks": 196,
                "num_produced_chunks": 784,
                "public_key": "ed25519:5ZyaXsGCya4Sch5bqUfohvo7iRFYB9ancRouggWRsiDU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2921120632046921271187128426400"
            },
            {
                "account_id": "stakesabai.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 184,
                "num_expected_chunks": 736,
                "num_produced_blocks": 184,
                "num_produced_chunks": 736,
                "public_key": "ed25519:6abauNvvWnEkagjVpWRy2tZJdzPkmqurUjteMTKk5KQF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2916599529707436502033624706018"
            },
            {
                "account_id": "lunanova.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 175,
                "num_expected_chunks": 700,
                "num_produced_blocks": 175,
                "num_produced_chunks": 700,
                "public_key": "ed25519:qkfP4NsSuHybdLhdvvYQ2Y9xWPsd249thEvrzbJBKNc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2622427399369414817186000302929"
            },
            {
                "account_id": "stardust.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 171,
                "num_expected_chunks": 684,
                "num_produced_blocks": 171,
                "num_produced_chunks": 684,
                "public_key": "ed25519:6rxCJpTnrT6NFuGg6d5Dj3FEUz1ScNU9u35ywB3dYhrX",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2553157941874787748569518739793"
            },
            {
                "account_id": "appload.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 175,
                "num_expected_chunks": 700,
                "num_produced_blocks": 175,
                "num_produced_chunks": 700,
                "public_key": "ed25519:6LbMVL6otkvZbpuC9sN3z7EXSMo3PT9noPeBdBZTFneM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2532426922468348624661109101590"
            },
            {
                "account_id": "republic.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 156,
                "num_expected_chunks": 624,
                "num_produced_blocks": 156,
                "num_produced_chunks": 624,
                "public_key": "ed25519:5sT6xtwxvLARW6y3KURYmyFd5SokJFhiK4jyqbamzzZ6",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2482584550374901873709806022455"
            },
            {
                "account_id": "fish.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 142,
                "num_expected_chunks": 568,
                "num_produced_blocks": 142,
                "num_produced_chunks": 568,
                "public_key": "ed25519:27KegJd17HeXHk9h5MqkT35QAuvYvo5GFgPTpSVU4kPN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2187792102672081557615815180041"
            },
            {
                "account_id": "jazza.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 127,
                "num_expected_chunks": 508,
                "num_produced_blocks": 127,
                "num_produced_chunks": 508,
                "public_key": "ed25519:EW66Fkv7XcE9FiybuYtVURjHhYeEgwWWpzF685Vi7foY",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1871713157812549329986725980819"
            },
            {
                "account_id": "moonlet.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 110,
                "num_expected_chunks": 440,
                "num_produced_blocks": 110,
                "num_produced_chunks": 440,
                "public_key": "ed25519:GkDwzPckMfhkdYgyFG69Uph8RJ12BcV9xNeZW2q93ZJD",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1815865529210119231347115946473"
            },
            {
                "account_id": "01node.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 99,
                "num_expected_chunks": 396,
                "num_produced_blocks": 99,
                "num_produced_chunks": 396,
                "public_key": "ed25519:5xz7EbcnPqabwoFezdJBxieK8S7XLsdHHuLwM4vLLhFt",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1747341167993947423171010648692"
            },
            {
                "account_id": "inotel.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 107,
                "num_expected_chunks": 428,
                "num_produced_blocks": 107,
                "num_produced_chunks": 428,
                "public_key": "ed25519:DmEDRntb9NwfbfdvDf6wzjsw1vxzQcJAAhFL2J75iLwr",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1678105108194287525338752445839"
            },
            {
                "account_id": "fresh.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 75,
                "num_expected_chunks": 300,
                "num_produced_blocks": 75,
                "num_produced_chunks": 300,
                "public_key": "ed25519:6YHLXhohY8kMnkp5Jw4HrJ52xtdyt1rcP6AaWkKzh3ED",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1188986838549746093756283676487"
            },
            {
                "account_id": "zkv_staketosupportprivacy.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 77,
                "num_expected_chunks": 308,
                "num_produced_blocks": 77,
                "num_produced_chunks": 308,
                "public_key": "ed25519:2kAo86DW8mDaLDg37rFhQY8UYSZVq1CtegUHBEDvpSMA",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1141163771500958000798214011610"
            },
            {
                "account_id": "staking_opp_disc.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 50,
                "num_expected_chunks": 200,
                "num_produced_blocks": 50,
                "num_produced_chunks": 200,
                "public_key": "ed25519:8XbCfLQVSwtwaBajvByG87CxPPbaFdryz5qEkde1fSGv",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "944538613860133661128979213636"
            },
            {
                "account_id": "qbit.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 46,
                "num_expected_chunks": 184,
                "num_produced_blocks": 46,
                "num_produced_chunks": 184,
                "public_key": "ed25519:5DqZLnDu6PMEyhJzc5NhiMsoWeYMWG1bC4AULyafoXMv",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "607210666689378782480957163067"
            },
            {
                "account_id": "p2p-org.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 35,
                "num_expected_chunks": 140,
                "num_produced_blocks": 35,
                "num_produced_chunks": 140,
                "public_key": "ed25519:J441YAvvYvjWs3aVzjc5KLLWRzmhQTEMaymPyWFkMGeG",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "533225044254527493001696041429"
            },
            {
                "account_id": "galaxydigital.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 31,
                "num_expected_chunks": 124,
                "num_produced_blocks": 31,
                "num_produced_chunks": 124,
                "public_key": "ed25519:8ZD8CcSzSfVsYo7XyABHJsYcrpBE3EL5MwukoEfrNYMR",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "522775168768998399284781294045"
            },
            {
                "account_id": "lionstake.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 32,
                "num_expected_chunks": 128,
                "num_produced_blocks": 32,
                "num_produced_chunks": 128,
                "public_key": "ed25519:8kciZQy815tZooy7HPJkBq2cyEw9L7fbsWcmWLgwG4m3",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "508949425632685959642365104982"
            },
            {
                "account_id": "kosmos_and_p2p.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 27,
                "num_expected_chunks": 108,
                "num_produced_blocks": 27,
                "num_produced_chunks": 108,
                "public_key": "ed25519:41GWxdQHe4Y2fuisvz5k5G2NwDFEavRkisoZkB5tfJuC",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "449634001393248382545917077917"
            },
            {
                "account_id": "prophet.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 30,
                "num_expected_chunks": 120,
                "num_produced_blocks": 30,
                "num_produced_chunks": 120,
                "public_key": "ed25519:BV5b4DpgCUy1TEitE4TVPhpTY7uDNpHc8DBPyH6cYCBq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "410382369439084656067474926216"
            },
            {
                "account_id": "vortex_live.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 28,
                "num_expected_chunks": 112,
                "num_produced_blocks": 28,
                "num_produced_chunks": 112,
                "public_key": "ed25519:GrPW17VhMVLi15JohsM2ag2GpcqpQuJNm3Hf6vPYXRYZ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "406105409496765546085624464809"
            },
            {
                "account_id": "centurion.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 44,
                "num_expected_chunks": 176,
                "num_produced_blocks": 44,
                "num_produced_chunks": 176,
                "public_key": "ed25519:66eogeJGkWhoipU3YE3QapJbvYRXze6rg4BE6g7kDBRk",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "395812839347735611500991363365"
            },
            {
                "account_id": "sparkpool.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 19,
                "num_expected_chunks": 76,
                "num_produced_blocks": 19,
                "num_produced_chunks": 76,
                "public_key": "ed25519:4GdDoLduepfbMCD9M3UUQ1jedRHv4cWWn6VEkoax8dT2",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "344364382012055070787767281876"
            },
            {
                "account_id": "binancestaking.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 19,
                "num_expected_chunks": 76,
                "num_produced_blocks": 19,
                "num_produced_chunks": 76,
                "public_key": "ed25519:H9o1RgTXZjBwD5GUEajbHy6S7UoeNYMwsqueCeadkHPH",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "279671931204692448342528165808"
            },
            {
                "account_id": "dexagon.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 18,
                "num_expected_chunks": 72,
                "num_produced_blocks": 18,
                "num_produced_chunks": 72,
                "public_key": "ed25519:AQHwptR3Ho348BpFXJDjkxpWMW5ZwN7xWM3XWAWSEEgs",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "277755655572878285447071183009"
            },
            {
                "account_id": "pathrocknetwork.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 17,
                "num_expected_chunks": 68,
                "num_produced_blocks": 17,
                "num_produced_chunks": 68,
                "public_key": "ed25519:2iJQLVXubWafG7K1NzGVvjP54UJCgVg3cuPMktw8r7uQ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "274077116771264804868259334465"
            },
            {
                "account_id": "ib.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 24,
                "num_expected_chunks": 96,
                "num_produced_blocks": 24,
                "num_produced_chunks": 96,
                "public_key": "ed25519:8jeZyfvtTDGNyLVwLKEiCQZrq6J8hHLcV6bsDKZQ4iia",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "271856243904226418840360323938"
            },
            {
                "account_id": "cryptogarik.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 22,
                "num_expected_chunks": 88,
                "num_produced_blocks": 22,
                "num_produced_chunks": 88,
                "public_key": "ed25519:45zFAC8pLgwn1d5pSBpBHesWbzngfRgd92zaom7K8m8j",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "263881217999373393218480831862"
            },
            {
                "account_id": "infiniteloop.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 17,
                "num_expected_chunks": 68,
                "num_produced_blocks": 17,
                "num_produced_chunks": 68,
                "public_key": "ed25519:9BUwtDegzwKcmJBjLgUDLHc3pePgPKcWJXYGcZb33Nyr",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "255712580646621863716049239943"
            },
            {
                "account_id": "pandateam.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 13,
                "num_expected_chunks": 52,
                "num_produced_blocks": 13,
                "num_produced_chunks": 52,
                "public_key": "ed25519:Cu83NRziNLiT6HLu9kJ8svFoftZQ9wVmjScxjqCybppt",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "246315500545919784372491775656"
            },
            {
                "account_id": "optimusvalidatornetwork.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 15,
                "num_expected_chunks": 60,
                "num_produced_blocks": 15,
                "num_produced_chunks": 60,
                "public_key": "ed25519:C3CJMKaWdEzkqyNCKwnKud6wDNnzs7Ura63k16zm4LUU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "239073862281816644196084546516"
            },
            {
                "account_id": "cryptoblossom.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 10,
                "num_expected_chunks": 40,
                "num_produced_blocks": 10,
                "num_produced_chunks": 40,
                "public_key": "ed25519:5opTNJEkCBYuyMgAghY2Sxp4bBtXYQtbEvZ3Wc5Awohb",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "238495868578085951517068741592"
            },
            {
                "account_id": "ledgerbyfigment.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 17,
                "num_expected_chunks": 68,
                "num_produced_blocks": 17,
                "num_produced_chunks": 68,
                "public_key": "ed25519:4JJTNeMaSb8W3NELh2rkkrDCqG1VpM3gdJ1hc9HFTBmN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "206435950524585528987715294084"
            },
            {
                "account_id": "incrypted.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 11,
                "num_expected_chunks": 44,
                "num_produced_blocks": 11,
                "num_produced_chunks": 44,
                "public_key": "ed25519:CsnkDDxNP6ukieSgz31dz9rA3UDKamKB2So2iABVhubi",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "198621123094637125815006247701"
            },
            {
                "account_id": "ni.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 12,
                "num_expected_chunks": 48,
                "num_produced_blocks": 12,
                "num_produced_chunks": 48,
                "public_key": "ed25519:8sRAjT6nFnCtGmppKXFuwqvRre5EPspZCLncFc5Aok7z",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "197633690311970966093037905293"
            },
            {
                "account_id": "stakely_io.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 12,
                "num_expected_chunks": 48,
                "num_produced_blocks": 12,
                "num_produced_chunks": 48,
                "public_key": "ed25519:HWp9E3gP91s25ddMS9xUWuzbJUpVGiPoitu5bT6hqMHs",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "196529887010171557157352777645"
            },
            {
                "account_id": "shardlabs.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 10,
                "num_expected_chunks": 40,
                "num_produced_blocks": 10,
                "num_produced_chunks": 40,
                "public_key": "ed25519:Gj5ToPBT4Ygh6CFT654bf1Y2FkWQAA7KFNCkeRGEV4VB",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "193402940014492944684002894771"
            },
            {
                "account_id": "grassets.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 16,
                "num_expected_chunks": 64,
                "num_produced_blocks": 16,
                "num_produced_chunks": 64,
                "public_key": "ed25519:GS8uhr7mhsBWB5c1JgvsJzpwZDGrcnB9Xnw7YRyMSQP5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "191901227764248254880229485940"
            },
            {
                "account_id": "staking-power.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 11,
                "num_expected_chunks": 44,
                "num_produced_blocks": 11,
                "num_produced_chunks": 44,
                "public_key": "ed25519:42ikqyV1BYmSnhHJ9EsLLy9kgeAg1mC3qqU1AJGaTEaW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "189415403495017120460053988282"
            },
            {
                "account_id": "bflame.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 12,
                "num_expected_chunks": 48,
                "num_produced_blocks": 12,
                "num_produced_chunks": 48,
                "public_key": "ed25519:6QDZab171amvZ8ZP3k2UqiwqcYBBD3HjC3ErYJ7ndWCK",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "187971327630135670600710452556"
            },
            {
                "account_id": "inc4.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 17,
                "num_expected_chunks": 68,
                "num_produced_blocks": 17,
                "num_produced_chunks": 68,
                "public_key": "ed25519:EPK4Cnkuua9vH75Rq5f6r66fcfR6eFi5pS3o5iiV7hKP",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "186102075929445580093434071621"
            },
            {
                "account_id": "doubletop.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 10,
                "num_expected_chunks": 40,
                "num_produced_blocks": 10,
                "num_produced_chunks": 40,
                "public_key": "ed25519:G5YQUqsVJd1qR2N7tQsxuZGW6izE6Kx8i2F5fDVKUJ39",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "183613871770328520878753472307"
            },
            {
                "account_id": "genesislab.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 15,
                "num_expected_chunks": 60,
                "num_produced_blocks": 15,
                "num_produced_chunks": 60,
                "public_key": "ed25519:Do8QywDQ9DBvHaoxSwzAhuejv3ZU8CFkQ9xWWnHVaQRM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "180032818054154062119032862631"
            },
            {
                "account_id": "sicmundus.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 15,
                "num_expected_chunks": 60,
                "num_produced_blocks": 15,
                "num_produced_chunks": 60,
                "public_key": "ed25519:Fh4pUKGsCVqutYHS52RLCA7UpLaCVWF5LZ9xXo94zQBw",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "178899403255786687156604156952"
            },
            {
                "account_id": "4ire.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 10,
                "num_expected_chunks": 40,
                "num_produced_blocks": 10,
                "num_produced_chunks": 40,
                "public_key": "ed25519:GdirfFSuT3t1ChEMqwcV6zko5Ya9yVAqm6Pnhk9qcXvS",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "178646417468115806102982413251"
            },
            {
                "account_id": "lavenderfive.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 13,
                "num_expected_chunks": 52,
                "num_produced_blocks": 13,
                "num_produced_chunks": 52,
                "public_key": "ed25519:HXiLVGFiMssLHH6H36G7AsaYhBankPNgd4b7uNsXzQVF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "177873750362635129983693343754"
            },
            {
                "account_id": "dariya.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 5,
                "num_expected_chunks": 20,
                "num_produced_blocks": 5,
                "num_produced_chunks": 20,
                "public_key": "ed25519:AJc9P74HBXGas6mqpA8XJDWgNzM9ZLxYiH6q7cdY75pn",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "176590798288073866093227388480"
            },
            {
                "account_id": "stakesstone.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 6,
                "num_expected_chunks": 24,
                "num_produced_blocks": 6,
                "num_produced_chunks": 24,
                "public_key": "ed25519:crXSnXFFbBr3eCXPeV54bUPm6m4D4EYgLzUmxM2G9FU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "176197055190562629921889037972"
            },
            {
                "account_id": "anchikovproduction.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 10,
                "num_expected_chunks": 40,
                "num_produced_blocks": 10,
                "num_produced_chunks": 40,
                "public_key": "ed25519:HMhR7VGBwC4GDyDpDRrgdArvCXmjhEvgu2X7iiCnikTJ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "175986273914768250300505167848"
            },
            {
                "account_id": "galactic.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 12,
                "num_expected_chunks": 48,
                "num_produced_blocks": 12,
                "num_produced_chunks": 48,
                "public_key": "ed25519:GFK83N32DbERtFg8rkpfNBsKtkFpmNQzyKFM9kJvPCMG",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "173476859866723770564738378414"
            },
            {
                "account_id": "avado.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 9,
                "num_expected_chunks": 36,
                "num_produced_blocks": 9,
                "num_produced_chunks": 36,
                "public_key": "ed25519:FdLWsf42e3Sc7bdKMtxJMgWRP21ysZDSXFnS2vTwTaaA",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "115675823336794834530400782890"
            },
            {
                "account_id": "steak.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 4,
                "num_expected_chunks": 16,
                "num_produced_blocks": 4,
                "num_produced_chunks": 16,
                "public_key": "ed25519:3tZG4QgzWpTKt2dChqZVUTBvF35pvG7BHyyJULF8VXQc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "111777740647836506266678052462"
            },
            {
                "account_id": "near-fans.poolv1.near",
                "is_slashed": false,
                "num_expected_blocks": 4,
                "num_expected_chunks": 16,
                "num_produced_blocks": 4,
                "num_produced_chunks": 16,
                "public_key": "ed25519:AgV97ssnHm7qN8JhYZjwyDtuaT6Ms3Fgbw3WeAC8M3iF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "109161832795081029944906907656"
            }
        ],
        "epoch_height": 1228,
        "epoch_start_height": 62869882,
        "next_fishermen": [],
        "next_validators": [
            {
                "account_id": "staked.poolv1.near",
                "public_key": "ed25519:3JBVXqenru2ErAM1kHQ8qfd29dCkURLd6JKrFgtmcDTZ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "43368226757335281618630692177771"
            },
            {
                "account_id": "astro-stakers.poolv1.near",
                "public_key": "ed25519:2nPSBCzjqikgwrqUMcuEVReJhmkC91eqJGPGqH9sZc28",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "24359644862759716866969996472023"
            },
            {
                "account_id": "bzam6yjpnfnxsdmjf6pw.poolv1.near",
                "public_key": "ed25519:2ZJqaaCAisK4u8E2i611zFfvNmrvevovnU3M7SpGHkLY",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "23585103803100053583804199195074"
            },
            {
                "account_id": "bisontrails.poolv1.near",
                "public_key": "ed25519:Emk6wQJtpQZRJCvvPmmwP9GD2Pk37xxRpmb5uRvJpX62",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "20640403103723076674179600952045"
            },
            {
                "account_id": "dragonfly.poolv1.near",
                "public_key": "ed25519:6Gj8MRp9KqfdiXa35LJcZnqeBNNEZoYk6ysvpzHaruvq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "19851064797934609781507555517222"
            },
            {
                "account_id": "foundry.poolv1.near",
                "public_key": "ed25519:5Qx8Fq3SK4Vu1sRRpf2HsNGLAqdNqgkKEebHMniLWhkW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "19198992750142358014914183170052"
            },
            {
                "account_id": "aurora.pool.near",
                "public_key": "ed25519:FZKXoWHFCXMrKiXjAKFdHo5g9PDom4bWMRFERBfufi2Y",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "17826118707687495886819812110506"
            },
            {
                "account_id": "finoa.poolv1.near",
                "public_key": "ed25519:62gxgzoie7FiK9dnWuiwM1bbuvhpceYDavK7SgdfEMJc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "14114754668854203092126047854510"
            },
            {
                "account_id": "epic.poolv1.near",
                "public_key": "ed25519:68HExKDtw1CjGzopZ8fMAMhMSZRVKRhwLzLQmGKtFNzT",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "11544086572008890493139702267616"
            },
            {
                "account_id": "magic.poolv1.near",
                "public_key": "ed25519:5fwufMXx9CTyLRkz7x3htQa3rFGzFZuz6d43LhCTmKCS",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "10521762585393711695165177620301"
            },
            {
                "account_id": "zavodil.poolv1.near",
                "public_key": "ed25519:HHARoU1hANWF9hu7YRstDDvgyigBhUeUuqecRVr8dpUz",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9893485720225071919263722701590"
            },
            {
                "account_id": "electric.poolv1.near",
                "public_key": "ed25519:GpSr5KAZMZ1Cb4dHMRUVhmp95y2fmWtm4dEjAr8iAva5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9757452719762401390818144342863"
            },
            {
                "account_id": "rekt.poolv1.near",
                "public_key": "ed25519:FoAaUdVKEHtVokG1aVmJNou61YcfQhXmaZ5Hnfsz4fHC",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9417333611593529135295059165997"
            },
            {
                "account_id": "stake1.poolv1.near",
                "public_key": "ed25519:7EiVt9i7SmULDKEnAXBFSMzwUmZdxUYDFkP73MZuCH1h",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "9361363077529080562198877045689"
            },
            {
                "account_id": "d1.poolv1.near",
                "public_key": "ed25519:7ZhMRwnSHGJtWjGBZiRhhSi6XyqKeNHtnEXsVTNdrsk6",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "7233513291182467474710960258828"
            },
            {
                "account_id": "nearcrowd.poolv1.near",
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "7068212655644200626637902216043"
            },
            {
                "account_id": "blockdaemon.poolv1.near",
                "public_key": "ed25519:3GNFSJiFQQ1rnR68T4eZRff2omPhg1CTewUHBJpQAdyc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "6819329727691872486048873004838"
            },
            {
                "account_id": "anonymous.poolv1.near",
                "public_key": "ed25519:Hoj7LbPwNwAkLFhf8z2aDF1BG6NDSrq1BfkdaKqPfbXx",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "6258409764546154833599639541787"
            },
            {
                "account_id": "dokiacapital.poolv1.near",
                "public_key": "ed25519:FGcJJeWMyx1xDbfkcPM2oMeUeGaADJuPmeqx5rjsHn7t",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5898604626587132249307306443345"
            },
            {
                "account_id": "08investinwomen_runbybisontrails.poolv1.near",
                "public_key": "ed25519:C6yqxQ3suwjmm8ufG5e3BsHiwxUs9h839FCneF41V7TM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5528385303149236680141401320797"
            },
            {
                "account_id": "chorusone.poolv1.near",
                "public_key": "ed25519:AZwJAgu2qRxHwdpj8ioZEFGcc2jbaZGN7ZvUe7CuXtM7",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5468852407838727923674080115061"
            },
            {
                "account_id": "binancenode1.poolv1.near",
                "public_key": "ed25519:Bb7uPEocbsiQwRfPmsiiiM88DodtuYnBDi6dKZ4JZo2N",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5335417765518321142946998509622"
            },
            {
                "account_id": "accomplice.poolv1.near",
                "public_key": "ed25519:5ck255MtkoGQxh9LfjNtdb4M7WHkUmjU7SBJCEkZP2B7",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5257121806135739838206200800745"
            },
            {
                "account_id": "abl_pool.poolv1.near",
                "public_key": "ed25519:5nnwJr7WgMXbWiudFcen9AMXRUXWA3ij6GGFZvRWXA3C",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5235606465132875209202784721942"
            },
            {
                "account_id": "future_is_near.poolv1.near",
                "public_key": "ed25519:F3vEGwYYGisaXwKJWrYgorB95DfArDby8bK5wydxD5fp",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5162135220955100348906007910716"
            },
            {
                "account_id": "legends.poolv1.near",
                "public_key": "ed25519:DNK46DeHKeJPF9YetmNxZnqtpkeLjdUb9ezSRCue3TpB",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "5022407163554559495728420351563"
            },
            {
                "account_id": "hb436_pool.poolv1.near",
                "public_key": "ed25519:7oU4C3vWqkeup7aMfjyV1ojt7yKX7ShLfvNCahBRy1eW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4907444704305182864018741022770"
            },
            {
                "account_id": "continue.poolv1.near",
                "public_key": "ed25519:9rDZywYL3tnvzj6hnePw3MaPFPfSeSCLxBp1niTGbMaK",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4756491050663638835709293112582"
            },
            {
                "account_id": "openshards.poolv1.near",
                "public_key": "ed25519:4Xm73PiAGMZu3mZg4gF7j96iTAFHGbPvqzxBaTgKP4ub",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4507968350393156681801255198235"
            },
            {
                "account_id": "figment.poolv1.near",
                "public_key": "ed25519:7RjyY1bRKDqkshbKZtgpQdwsdxou8j9my8g1hPKZ9ngM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4479743505170227818938893243637"
            },
            {
                "account_id": "ideocolabventures.poolv1.near",
                "public_key": "ed25519:6NFuvrmnJiokXibR9Z7TUHjB4NJnD1rJAHhBu9JWmBdh",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4461246909283749795547935680284"
            },
            {
                "account_id": "northernlights.poolv1.near",
                "public_key": "ed25519:7HXh6iS9Rh92Uj1c5T9fPjQXPLnti4Rr2cJQcJEYpdGV",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4356664106365568775235422080785"
            },
            {
                "account_id": "buildlinks.poolv1.near",
                "public_key": "ed25519:Hd3irGt4zEqRPAzcFszX3oTkVWRFFxdecDvShCJSS1Wg",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4143098665113447616802571808129"
            },
            {
                "account_id": "nc2.poolv1.near",
                "public_key": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "4129184961008612084540404361177"
            },
            {
                "account_id": "smart-stake.poolv1.near",
                "public_key": "ed25519:A6wpkLQiYqPZ1rbd9s5S1Bg3LxccVsQqiCRDUXwzJ6Hx",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3896963297174413395315355197511"
            },
            {
                "account_id": "pandora.poolv1.near",
                "public_key": "ed25519:53N7KBhSkEP6tLuQmxZV9fAK16D1C2kWnuzes8KNyS7P",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3793881581979110196824343570298"
            },
            {
                "account_id": "stakin.poolv1.near",
                "public_key": "ed25519:85UGfKdVoxX9u86JsBMxmVHBguYonnM3vTR2WoD5GkEg",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3785048877627792390003879076232"
            },
            {
                "account_id": "nearfans.poolv1.near",
                "public_key": "ed25519:GM8vWM4TqTt7jh3sXYCAs2KPyn4vEmAceteBGEFYhyku",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3611677710987010058938838499944"
            },
            {
                "account_id": "erm.poolv1.near",
                "public_key": "ed25519:88nnN6LAuCbJaj9wucd1WUMfTtdv2s3njpvozHft8oQ5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3579477620025314874929633368972"
            },
            {
                "account_id": "nodeasy.poolv1.near",
                "public_key": "ed25519:8mjespqqUePSYSsxYxPqCUsZUuMxVJr1vjBRwFeCke5K",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3551854680420926041007904575021"
            },
            {
                "account_id": "cryptium.poolv1.near",
                "public_key": "ed25519:5Y9hW8cKBb5RnsJBqttHHC5ujz5zcZZ5xnrJPwkCWmGQ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3500807550656100196086753212997"
            },
            {
                "account_id": "lux.poolv1.near",
                "public_key": "ed25519:HzTGTDfTz63QGvvUdMGozFeaENFGyYAoSrqYJb23qZFN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3338883640902469506257972347265"
            },
            {
                "account_id": "everstake.poolv1.near",
                "public_key": "ed25519:4JLvwa1r2eAxHLyKeDJnpqMG5f2Z9rr49rwuTwb9g8u2",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3338315190933498625640678233294"
            },
            {
                "account_id": "sharpdarts.poolv1.near",
                "public_key": "ed25519:9XMHXqv7rM3QQxzjUu7dfKD7GhMkq8CEceaPdkhiBQUX",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3237308983457011676954090848755"
            },
            {
                "account_id": "dsrvlabs.poolv1.near",
                "public_key": "ed25519:9SACdsDDgXA2WZLfJvpkKbu22Exxtc4CMbeHmVnN2P4a",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3076761509244926826309981029293"
            },
            {
                "account_id": "hashquark.poolv1.near",
                "public_key": "ed25519:3YDdmN1vhF7yAWnYxGMHY46jcLE9h11HvEeF6Kntugeq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "3049883042641669172552391988824"
            },
            {
                "account_id": "baziliknear.poolv1.near",
                "public_key": "ed25519:E4LAWdgLifBEoaWvhRNy5vpdAnUc3GsUHePeiAurZY5v",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2993267214992126150787644838403"
            },
            {
                "account_id": "stakesabai.poolv1.near",
                "public_key": "ed25519:6abauNvvWnEkagjVpWRy2tZJdzPkmqurUjteMTKk5KQF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2931754524247171975709619856295"
            },
            {
                "account_id": "masternode24.poolv1.near",
                "public_key": "ed25519:5ZyaXsGCya4Sch5bqUfohvo7iRFYB9ancRouggWRsiDU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2931090209993204168348616061404"
            },
            {
                "account_id": "lunanova.poolv1.near",
                "public_key": "ed25519:qkfP4NsSuHybdLhdvvYQ2Y9xWPsd249thEvrzbJBKNc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2631187952956768543634382212447"
            },
            {
                "account_id": "stardust.poolv1.near",
                "public_key": "ed25519:6rxCJpTnrT6NFuGg6d5Dj3FEUz1ScNU9u35ywB3dYhrX",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2566198484149698450713817673017"
            },
            {
                "account_id": "appload.poolv1.near",
                "public_key": "ed25519:6LbMVL6otkvZbpuC9sN3z7EXSMo3PT9noPeBdBZTFneM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2544994434001273053710958003170"
            },
            {
                "account_id": "republic.poolv1.near",
                "public_key": "ed25519:5sT6xtwxvLARW6y3KURYmyFd5SokJFhiK4jyqbamzzZ6",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2483064257228690921326320594647"
            },
            {
                "account_id": "fish.poolv1.near",
                "public_key": "ed25519:27KegJd17HeXHk9h5MqkT35QAuvYvo5GFgPTpSVU4kPN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "2195982706548604434757753562270"
            },
            {
                "account_id": "jazza.poolv1.near",
                "public_key": "ed25519:EW66Fkv7XcE9FiybuYtVURjHhYeEgwWWpzF685Vi7foY",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1880584405976725049625149745285"
            },
            {
                "account_id": "moonlet.poolv1.near",
                "public_key": "ed25519:GkDwzPckMfhkdYgyFG69Uph8RJ12BcV9xNeZW2q93ZJD",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1816295057556463487053800731314"
            },
            {
                "account_id": "01node.poolv1.near",
                "public_key": "ed25519:5xz7EbcnPqabwoFezdJBxieK8S7XLsdHHuLwM4vLLhFt",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1761802988107026742428566410241"
            },
            {
                "account_id": "inotel.poolv1.near",
                "public_key": "ed25519:DmEDRntb9NwfbfdvDf6wzjsw1vxzQcJAAhFL2J75iLwr",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1689266910220114910366972936356"
            },
            {
                "account_id": "fresh.poolv1.near",
                "public_key": "ed25519:6YHLXhohY8kMnkp5Jw4HrJ52xtdyt1rcP6AaWkKzh3ED",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1202718640732944316307448342909"
            },
            {
                "account_id": "zkv_staketosupportprivacy.poolv1.near",
                "public_key": "ed25519:2kAo86DW8mDaLDg37rFhQY8UYSZVq1CtegUHBEDvpSMA",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "1148062514858698697929925514593"
            },
            {
                "account_id": "staking_opp_disc.poolv1.near",
                "public_key": "ed25519:8XbCfLQVSwtwaBajvByG87CxPPbaFdryz5qEkde1fSGv",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "944721055570181744656380258076"
            },
            {
                "account_id": "qbit.poolv1.near",
                "public_key": "ed25519:5DqZLnDu6PMEyhJzc5NhiMsoWeYMWG1bC4AULyafoXMv",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "616847596492586061257316266304"
            },
            {
                "account_id": "p2p-org.poolv1.near",
                "public_key": "ed25519:J441YAvvYvjWs3aVzjc5KLLWRzmhQTEMaymPyWFkMGeG",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "550841575079944059966217859964"
            },
            {
                "account_id": "galaxydigital.poolv1.near",
                "public_key": "ed25519:8ZD8CcSzSfVsYo7XyABHJsYcrpBE3EL5MwukoEfrNYMR",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "522877645795935631305631753454"
            },
            {
                "account_id": "lionstake.poolv1.near",
                "public_key": "ed25519:8kciZQy815tZooy7HPJkBq2cyEw9L7fbsWcmWLgwG4m3",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "509037122315834737322138953169"
            },
            {
                "account_id": "kosmos_and_p2p.poolv1.near",
                "public_key": "ed25519:41GWxdQHe4Y2fuisvz5k5G2NwDFEavRkisoZkB5tfJuC",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "449820529935873803936255722725"
            },
            {
                "account_id": "prophet.poolv1.near",
                "public_key": "ed25519:BV5b4DpgCUy1TEitE4TVPhpTY7uDNpHc8DBPyH6cYCBq",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "424662637430574665816126694316"
            },
            {
                "account_id": "vortex_live.poolv1.near",
                "public_key": "ed25519:GrPW17VhMVLi15JohsM2ag2GpcqpQuJNm3Hf6vPYXRYZ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "414310873767067739372194487896"
            },
            {
                "account_id": "centurion.poolv1.near",
                "public_key": "ed25519:66eogeJGkWhoipU3YE3QapJbvYRXze6rg4BE6g7kDBRk",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "409497036160351441587073011745"
            },
            {
                "account_id": "sparkpool.poolv1.near",
                "public_key": "ed25519:4GdDoLduepfbMCD9M3UUQ1jedRHv4cWWn6VEkoax8dT2",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "344428294366082125643976278017"
            },
            {
                "account_id": "dexagon.poolv1.near",
                "public_key": "ed25519:AQHwptR3Ho348BpFXJDjkxpWMW5ZwN7xWM3XWAWSEEgs",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "291349384880267686316797413919"
            },
            {
                "account_id": "pathrocknetwork.poolv1.near",
                "public_key": "ed25519:2iJQLVXubWafG7K1NzGVvjP54UJCgVg3cuPMktw8r7uQ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "285779615436826804944566663893"
            },
            {
                "account_id": "ib.poolv1.near",
                "public_key": "ed25519:8jeZyfvtTDGNyLVwLKEiCQZrq6J8hHLcV6bsDKZQ4iia",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "282741767857383431851441368281"
            },
            {
                "account_id": "binancestaking.poolv1.near",
                "public_key": "ed25519:H9o1RgTXZjBwD5GUEajbHy6S7UoeNYMwsqueCeadkHPH",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "279739376980933520560349653397"
            },
            {
                "account_id": "cryptogarik.poolv1.near",
                "public_key": "ed25519:45zFAC8pLgwn1d5pSBpBHesWbzngfRgd92zaom7K8m8j",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "276719770843148887778545288521"
            },
            {
                "account_id": "infiniteloop.poolv1.near",
                "public_key": "ed25519:9BUwtDegzwKcmJBjLgUDLHc3pePgPKcWJXYGcZb33Nyr",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "271919318661209546544580183542"
            },
            {
                "account_id": "pandateam.poolv1.near",
                "public_key": "ed25519:Cu83NRziNLiT6HLu9kJ8svFoftZQ9wVmjScxjqCybppt",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "258524418682763194348198260976"
            },
            {
                "account_id": "optimusvalidatornetwork.poolv1.near",
                "public_key": "ed25519:C3CJMKaWdEzkqyNCKwnKud6wDNnzs7Ura63k16zm4LUU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "253882667926738108795377479367"
            },
            {
                "account_id": "cryptoblossom.poolv1.near",
                "public_key": "ed25519:5opTNJEkCBYuyMgAghY2Sxp4bBtXYQtbEvZ3Wc5Awohb",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "250866274265207026084815238797"
            },
            {
                "account_id": "ledgerbyfigment.poolv1.near",
                "public_key": "ed25519:4JJTNeMaSb8W3NELh2rkkrDCqG1VpM3gdJ1hc9HFTBmN",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "214836197238893751665164285778"
            },
            {
                "account_id": "incrypted.poolv1.near",
                "public_key": "ed25519:CsnkDDxNP6ukieSgz31dz9rA3UDKamKB2So2iABVhubi",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "212856146584318123246812885924"
            },
            {
                "account_id": "stakely_io.poolv1.near",
                "public_key": "ed25519:HWp9E3gP91s25ddMS9xUWuzbJUpVGiPoitu5bT6hqMHs",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "208014198804983417689050261591"
            },
            {
                "account_id": "ni.poolv1.near",
                "public_key": "ed25519:8sRAjT6nFnCtGmppKXFuwqvRre5EPspZCLncFc5Aok7z",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "207662012458668060573875548513"
            },
            {
                "account_id": "doubletop.poolv1.near",
                "public_key": "ed25519:G5YQUqsVJd1qR2N7tQsxuZGW6izE6Kx8i2F5fDVKUJ39",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "194498601458119467292726196891"
            },
            {
                "account_id": "inc4.poolv1.near",
                "public_key": "ed25519:EPK4Cnkuua9vH75Rq5f6r66fcfR6eFi5pS3o5iiV7hKP",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "194497886850532525286307978298"
            },
            {
                "account_id": "shardlabs.poolv1.near",
                "public_key": "ed25519:Gj5ToPBT4Ygh6CFT654bf1Y2FkWQAA7KFNCkeRGEV4VB",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "193413785748379091292543246409"
            },
            {
                "account_id": "grassets.poolv1.near",
                "public_key": "ed25519:GS8uhr7mhsBWB5c1JgvsJzpwZDGrcnB9Xnw7YRyMSQP5",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "191923101670235090476961392277"
            },
            {
                "account_id": "staking-power.poolv1.near",
                "public_key": "ed25519:42ikqyV1BYmSnhHJ9EsLLy9kgeAg1mC3qqU1AJGaTEaW",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "189650717813527337713010322845"
            },
            {
                "account_id": "bflame.poolv1.near",
                "public_key": "ed25519:6QDZab171amvZ8ZP3k2UqiwqcYBBD3HjC3ErYJ7ndWCK",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "188007635697236483445132011362"
            },
            {
                "account_id": "stakesstone.poolv1.near",
                "public_key": "ed25519:crXSnXFFbBr3eCXPeV54bUPm6m4D4EYgLzUmxM2G9FU",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "187336393290669716673245276914"
            },
            {
                "account_id": "sicmundus.poolv1.near",
                "public_key": "ed25519:Fh4pUKGsCVqutYHS52RLCA7UpLaCVWF5LZ9xXo94zQBw",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "187058397409562060260347612306"
            },
            {
                "account_id": "lavenderfive.poolv1.near",
                "public_key": "ed25519:HXiLVGFiMssLHH6H36G7AsaYhBankPNgd4b7uNsXzQVF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "186399292089619130765033611364"
            },
            {
                "account_id": "anchikovproduction.poolv1.near",
                "public_key": "ed25519:HMhR7VGBwC4GDyDpDRrgdArvCXmjhEvgu2X7iiCnikTJ",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "184146665438765596291824537944"
            },
            {
                "account_id": "genesislab.poolv1.near",
                "public_key": "ed25519:Do8QywDQ9DBvHaoxSwzAhuejv3ZU8CFkQ9xWWnHVaQRM",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "179965764090055271648451204172"
            },
            {
                "account_id": "4ire.poolv1.near",
                "public_key": "ed25519:GdirfFSuT3t1ChEMqwcV6zko5Ya9yVAqm6Pnhk9qcXvS",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "178680613992802838379024738838"
            },
            {
                "account_id": "dariya.poolv1.near",
                "public_key": "ed25519:AJc9P74HBXGas6mqpA8XJDWgNzM9ZLxYiH6q7cdY75pn",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "176665902215810579496096826857"
            },
            {
                "account_id": "galactic.poolv1.near",
                "public_key": "ed25519:GFK83N32DbERtFg8rkpfNBsKtkFpmNQzyKFM9kJvPCMG",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "173511368361518149170632798553"
            },
            {
                "account_id": "near-fans.poolv1.near",
                "public_key": "ed25519:AgV97ssnHm7qN8JhYZjwyDtuaT6Ms3Fgbw3WeAC8M3iF",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "119977270228412897105244043270"
            },
            {
                "account_id": "steak.poolv1.near",
                "public_key": "ed25519:3tZG4QgzWpTKt2dChqZVUTBvF35pvG7BHyyJULF8VXQc",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "111810431100112702149898847828"
            },
            {
                "account_id": "projecttent.poolv1.near",
                "public_key": "ed25519:9qtkAbFDuAuEDLaGkAV5MHmFSKEtczuxDWYc2eKgXCx8",
                "shards": [
                    0,
                    1,
                    2,
                    3
                ],
                "stake": "106221371602909101938743096722"
            }
        ],
        "prev_epoch_kickout": [
            {
                "account_id": "avado.poolv1.near",
                "reason": {
                    "NotEnoughBlocks": {
                        "expected": 13,
                        "produced": 7
                    }
                }
            }
        ]
    }
}
```