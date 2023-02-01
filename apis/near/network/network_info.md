---
description: Returns the current state of node network connections (active peers, transmitted data, etc.)
---

# Network Info

### **Parameters**

- `method:` network_info
- `params:` []

### **Returns**

Returns the current state of node network connections (active peers, transmitted data, etc.)

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
  "method": "network_info",
  "params": []
}'
```

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": "11",
    "result": {
        "active_peers": [
            {
                "account_id": null,
                "addr": "34.141.176.200:24567",
                "id": "ed25519:PAdg8Rw77WsvoC4t2NdAbbWpFqmi1iAfPtG9ZDFhbK3"
            },
            {
                "account_id": null,
                "addr": "13.115.56.72:24567",
                "id": "ed25519:7V2yW5pVzdS7XK6s3zgL4cehUtSNGZHxNWrZarZPFZbB"
            },
            {
                "account_id": null,
                "addr": "20.207.200.131:24567",
                "id": "ed25519:CVnG3nYgDEn5GwKzDetE1iRrHo1v4aDSwnBPGdsALw7J"
            },
            {
                "account_id": null,
                "addr": "34.94.105.53:24567",
                "id": "ed25519:3F461ekoqE2S7dsbxjmANErat1LnT2erPdmkfgEmLf9s"
            },
            {
                "account_id": null,
                "addr": "34.94.172.74:24567",
                "id": "ed25519:23SFdgmCbyp5junyMPSaSotL8LQpGjuh5fmpRPPXVAe3"
            },
            {
                "account_id": null,
                "addr": "34.147.37.31:24567",
                "id": "ed25519:HkVStDGTmtfujDiY8rhNcNBxm9tviD1QRKVs6y2x839C"
            },
            {
                "account_id": null,
                "addr": "34.85.165.25:24567",
                "id": "ed25519:5cdgb2uU57qDTpbZ87oiaxBR1iX6VmGpgkXi8CLUwj4s"
            },
            {
                "account_id": null,
                "addr": "34.79.71.236:24567",
                "id": "ed25519:3ZeWvULGHAQiNNCJRwTUcfKPNTWJQzpeu9WNVF978rsU"
            },
            {
                "account_id": null,
                "addr": "34.91.52.248:24567",
                "id": "ed25519:8MvmovbbJ4PYNgMCpBwvQRA2P4ZbpEcZGHX1448G3Ehm"
            },
            {
                "account_id": null,
                "addr": "34.141.159.28:24567",
                "id": "ed25519:3Au9RtZKutnMw5GsQoBXm7c3miGZW4HtLeCNXRzDbpVQ"
            },
            {
                "account_id": null,
                "addr": "54.162.101.109:24567",
                "id": "ed25519:6yac8UUYvoKFDBDymNWZ8ZXSmU2d4C2N5w6uHV7GML37"
            },
            {
                "account_id": null,
                "addr": "35.229.151.121:24567",
                "id": "ed25519:FzJhX2KRyKuj5BrE1QjUXPjUXWz4Gt44mY4guMcS1LE1"
            },
            {
                "account_id": null,
                "addr": "46.137.198.252:24567",
                "id": "ed25519:9yyNBcDZJ8Ndo8KSdgfjdKKK2GpWNAcVEMZUYATHh8fE"
            },
            {
                "account_id": null,
                "addr": "35.204.182.184:24567",
                "id": "ed25519:FmCWvRqa7ahNwbVY3KAnnuuMor7fVDE23NLesuQtLo1Z"
            },
            {
                "account_id": null,
                "addr": "5.9.151.210:24567",
                "id": "ed25519:EoRLpoZgWs4tpkMzwp4LKGTNZXC7KGbTQCGo9C6icEWh"
            },
            {
                "account_id": null,
                "addr": "35.229.135.238:24567",
                "id": "ed25519:9uCm2SZYa9PabEMf9EoyK92hgMyt3STT6GwxY6EyVWnX"
            },
            {
                "account_id": null,
                "addr": "34.81.39.75:24567",
                "id": "ed25519:5uxaeXUtBk8jQGxdfhjPi7kQkhcpNeoYgzpCs3wcUivN"
            },
            {
                "account_id": null,
                "addr": "34.94.146.155:24567",
                "id": "ed25519:4Mk6hjDGoPjZTwtbYF56nxgwer6YXUNJk7PCQK9z1Nia"
            },
            {
                "account_id": null,
                "addr": "34.80.58.181:24567",
                "id": "ed25519:3ZoBdWb9nh22BK3jQu5azL3wfoeLb73RLEHkXCiEio6q"
            },
            {
                "account_id": null,
                "addr": "34.90.235.83:24567",
                "id": "ed25519:tWb9TVAytnZVcmL4YZPrne9r9xkqJddrU9zZLucw5TZ"
            },
            {
                "account_id": null,
                "addr": "35.245.197.196:24567",
                "id": "ed25519:6KgxccVAZi6UnxnhpMvegAtRXvQtebtwn75MR3xPrUQQ"
            },
            {
                "account_id": null,
                "addr": "142.132.128.234:24567",
                "id": "ed25519:3HS7YDQgpDmwosvvgNNPz6GmajF1Lg93RsruWhLAReE3"
            },
            {
                "account_id": null,
                "addr": "34.70.25.110:24567",
                "id": "ed25519:8UqdcmDSm5aVQmnshSnzetodWjZqNNirKGJV7ffd4NGx"
            },
            {
                "account_id": null,
                "addr": "18.219.223.23:24567",
                "id": "ed25519:8q73NkGGna3qJTAcQKrZNHQ9dwoZPLZQ95xdn3tfqX3H"
            },
            {
                "account_id": null,
                "addr": "104.199.135.126:24567",
                "id": "ed25519:7vWwt95kVPioK2yAySisf6d2PrKSMEj7DQGw9VayCmRG"
            },
            {
                "account_id": null,
                "addr": "3.123.136.229:24567",
                "id": "ed25519:5VgULjHdW25enRFsQVUsVuRdxC2QrcCEYR9wpWwVdjav"
            },
            {
                "account_id": null,
                "addr": "34.90.40.46:24567",
                "id": "ed25519:2wBkV5jw7VminBJ3fZpQHq8n9HutpfdgmVJJEmG63ZtT"
            },
            {
                "account_id": null,
                "addr": "3.18.160.209:24567",
                "id": "ed25519:A6LKXieTr7Pb9drXjLqEs29NnzXhLoSvLitKSkZh2Qdg"
            },
            {
                "account_id": null,
                "addr": "135.181.118.241:24567",
                "id": "ed25519:Dzag6h9RkB6QUjzcAZFiSULWSbAra6c2gxwmru43dK3G"
            },
            {
                "account_id": null,
                "addr": "13.230.47.132:24567",
                "id": "ed25519:DApC1qJBVkEpJmVvsEnMB97hWuDoBmhQYkZkvHhDRRQn"
            }
        ],
        "known_producers": [
            {
                "account_id": "binancenode1.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6yac8UUYvoKFDBDymNWZ8ZXSmU2d4C2N5w6uHV7GML37"
            },
            {
                "account_id": "stakin.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:AKcjFQHUCD7FQQ5pgfHywP75VU5nAiF3He9egaFMBB72"
            },
            {
                "account_id": "baziliknear.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6HBtiS73NrRUCrnKHLzParNBraGaT2NQRX5o51FYaVH9"
            },
            {
                "account_id": "dexagon.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6v3juNRvjGSDoauKNzQJunHv2ktPdEMj5s6zoZ6NEnqJ"
            },
            {
                "account_id": "pandora.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Fc8H5cCGQuybcP1smTVs4X6BQD4irrxeeasNYNJwWzjF"
            },
            {
                "account_id": "d1.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:D6U7ruGbBeoRu4NFTjyMA6vhYoEkHfFdM2MMWrkiwxWU"
            },
            {
                "account_id": "inc4.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8oHkBHxZtV51NbPLUBaLZpmQn945EZPEnfgapXZoeZ8C"
            },
            {
                "account_id": "bzam6yjpnfnxsdmjf6pw.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:HbbeXczyYg8RxjofCZev4Ti6F5MHq5fbgs3jr6mNJEf"
            },
            {
                "account_id": "rekt.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7fPwmfuDAAGLz8UG8oJC5Pv6zz2wAJ2RfVZTTFLV7aS8"
            },
            {
                "account_id": "doubletop.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:HkiQwJqd5AceuReSd2n8o79u89EVYwNCJ7CS19XPKKFW"
            },
            {
                "account_id": "steak.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4D8Udo88RMJUwgdPcf2VjPXvAyLQn12Q18TqLBhtqPra"
            },
            {
                "account_id": "accomplice.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:UeH6Q1wm6ENxH5LBCL8ghiEeXZS5q8ZtbyLPeMR5Mzm"
            },
            {
                "account_id": "cryptoblossom.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Dzag6h9RkB6QUjzcAZFiSULWSbAra6c2gxwmru43dK3G"
            },
            {
                "account_id": "epic.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5xom7GfT1oGSBdA7W9KHshbw81Bih5Fp7nLHiTofD7ak"
            },
            {
                "account_id": "zkv_staketosupportprivacy.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4Jfxjj7kmd5K6BgXFRpLBMdRajYhC73xeuTeQ3Cgr1sW"
            },
            {
                "account_id": "masternode24.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4b67kGsWfHXmxh6N6r6APHzf3h1NTicLGH9wjgRRmRvU"
            },
            {
                "account_id": "erm.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:HS8U2FMXow9sqaJKcQGzSbePccpEpz67ierKucQ6ePTS"
            },
            {
                "account_id": "hb436_pool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BWcYjaGM7AQrAGK6KmaYEf84ViFBiHarF5qRCV6o5MdT"
            },
            {
                "account_id": "blockdaemon.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:3GNFSJiFQQ1rnR68T4eZRff2omPhg1CTewUHBJpQAdyc"
            },
            {
                "account_id": "fish.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:QvPjf67yZ8w2WySej2U1LgAxdSz6LdN96GkW6j55kwZ"
            },
            {
                "account_id": "continue.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:3yUZib8KMncy6aXCEtpWoAE5VBvU4AHtQ6WLvTHaWtCF"
            },
            {
                "account_id": "cryptium.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:268mmTfy4oteCbzBY4HusxYZtDZaWdQaiM5HtTbQmtY5"
            },
            {
                "account_id": "kosmos_and_p2p.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:EKjZvdKiDFSo3R1vVyaZfgAQXQ1XhuoK2LXWGWArVQA"
            },
            {
                "account_id": "lunanova.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8waJfKqzU8P4w7rnzop3cRo6uM1u5vRrPPhN3MEn212j"
            },
            {
                "account_id": "nodeasy.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:25fSg2aqemEryuKBBByM3GDtCMZSyaQ7ZzfkJSPghx2Y"
            },
            {
                "account_id": "pathrocknetwork.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:A7mVYCR1DEeS84Vy8gtMdryPzTtUCtEwkJ5Hk6adoqg6"
            },
            {
                "account_id": "sparkpool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:83C8GonqG3PKkdt7gfexnU592aKGs3BfZhgeA8CSBJcS"
            },
            {
                "account_id": "pandateam.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:73iUsj3cLuU2tYgPj2wrycpNJNfkyACbT3rzGAJ1nuiS"
            },
            {
                "account_id": "foundry.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8q6P3DvzRMQeXBRr2TTRyEbGFScnF6DYb6CfRFusgbuZ"
            },
            {
                "account_id": "sicmundus.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:AsGReU5fC9bj1mEnfDUcEWFm9gca7TjXVC3F2AoHNurE"
            },
            {
                "account_id": "08investinwomen_runbybisontrails.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2KZcs3Kc8njbVCM6fzNeRZs28hKR1VAHDm8NB1hk8c8R"
            },
            {
                "account_id": "stakesabai.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Atbk4odY1ME5mk8SWgkjqfnWsFboWj1KeVwCeCPG3CaF"
            },
            {
                "account_id": "fresh.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5o8sX1MYjkWHpLNEW6j8mQjxDu9rJw68eCjUQcQddVLm"
            },
            {
                "account_id": "genesislab.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:DTZFKmne5V31iWqkPGUSusKWP44a36ixUq12RA2Jg2PV"
            },
            {
                "account_id": "cryptogarik.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7vgGDhjqpDPUEgi4AtyPG12CPXE87Us33U6zK3nch6vx"
            },
            {
                "account_id": "near-fans.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7Czfp1VuduayzhYr5mpbrxtgtaqB6CYWeTTunAbBwL8a"
            },
            {
                "account_id": "astro-stakers.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:FrbiAcqoV4ZrGXaSgf2faXgT6BSa3jRG1NWYvns8Kyho"
            },
            {
                "account_id": "p2p-org.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8zkHCEcEQ97kSZm45HZ6UymZLP2uHHY6eGVZ8kLpT14T"
            },
            {
                "account_id": "nearfans.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:3e1sLMH2fvpGoZLcJQEuvSm3wtit16nPZ2qGP3UUXZ2B"
            },
            {
                "account_id": "ledgerbyfigment.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:DbhYaAsuKsfgHwC6nmKxQ5tMaGgBxkkbynbsTKHQx5c"
            },
            {
                "account_id": "staking_opp_disc.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:9yyNBcDZJ8Ndo8KSdgfjdKKK2GpWNAcVEMZUYATHh8fE"
            },
            {
                "account_id": "dragonfly.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6Gj8MRp9KqfdiXa35LJcZnqeBNNEZoYk6ysvpzHaruvq"
            },
            {
                "account_id": "openshards.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:H62grQCpzfiB145i7u4CMn8ayx6gpGbHr75NykcmoWs1"
            },
            {
                "account_id": "nearcrowd.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:FXXrTXiKWpXj1R6r5fBvMLpstd8gPyrBq3qMByqKVzKF"
            },
            {
                "account_id": "stakely_io.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:36ErCQ5DGJF3oqW2dwRhKyrMGv6C2Yq46LQyNo862yBU"
            },
            {
                "account_id": "aurora.pool.near",
                "addr": null,
                "peer_id": "ed25519:8JcU5rx3feMtFarVBvTnJtd31TiU4aTzbZvcUsP9q8x7"
            },
            {
                "account_id": "staking-power.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5uyA8ZCGT1f8gPYok3uryuagRkqZXXakxQFYece5G4vN"
            },
            {
                "account_id": "buildlinks.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BpyJ5xeh5EYB2zVwzqGhjvSFSqKA7iDyaqjW32wDo3JM"
            },
            {
                "account_id": "incrypted.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Hp74AobcFkyKqDU7NZQAhqbvHTesouRCveCFWfEe6NAp"
            },
            {
                "account_id": "chorusone.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:58prL2mSbiNSGLw6HnN9Y18zCmeVZARcsAGAjYwzsgGF"
            },
            {
                "account_id": "centurion.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:CVnG3nYgDEn5GwKzDetE1iRrHo1v4aDSwnBPGdsALw7J"
            },
            {
                "account_id": "hashquark.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5pRiNCHbXFALoVqHJtqvUdJadT85r6L3GVSnyUeS3GJX"
            },
            {
                "account_id": "dsrvlabs.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6oSQBoaLLR2ttvqbPAEVT5TKfwYUyi3qYu7CXA5B5ERV"
            },
            {
                "account_id": "optimusvalidatornetwork.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4x3nCXnkqMoyDNndPcnP239pqBLQzcawK6MQHpABmM5X"
            },
            {
                "account_id": "vortex_live.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:D3o7BwYRY4UgWe9RcJXRAgCDYRcHLWkR77qEm3LWyjJi"
            },
            {
                "account_id": "staked.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Gz76mL1D77d1nDZQi1jZM6WwdH8QEAHt3sor2khaFQLs"
            },
            {
                "account_id": "smart-stake.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:FDDPZ6ujJAv7ojQkBWsXLCQQNKkNXz29PejjPNgrQQgr"
            },
            {
                "account_id": "dariya.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:3k4m5miQtfHZYid9rg2nioWTK8rdkSqcruCwsFm6FLH6"
            },
            {
                "account_id": "jazza.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:J5hTXUMkk4zEi6wK1jtN1XeMak9oxwkme3cW5K6ZnFQs"
            },
            {
                "account_id": "magic.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:FPmhXppyWeNfDgSeA3jYxLxdGvDgR8QYdnhdZB4AuEN5"
            },
            {
                "account_id": "bflame.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:DqbNjrDjpr5jFvzA2SebAyGQTS1DUJULZmfhzXygfL6H"
            },
            {
                "account_id": "figment.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:J5Ls6pUiMZMc7VvZY7EZ2wRAyZdjfy1xqP7zZGtBvoKq"
            },
            {
                "account_id": "grassets.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:EJexoHcejVWzimZZ7KR4cKhf37Uz6XNGRocsneAhDMU6"
            },
            {
                "account_id": "binancestaking.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:9ravz6YFcUhcM6w6s2DPoBhWHmr4rAJNSLQvPNgQcFHE"
            },
            {
                "account_id": "inotel.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:CKrqFy8Ma5qjnMasNhqURpx6M7qFFaTVLb5XVEWGzXMB"
            },
            {
                "account_id": "prophet.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4UdKij8s71cKCqYHAwUapwsfZ9dbh1cDfCBfya8UxQbW"
            },
            {
                "account_id": "stardust.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:99McpjBiHTxYdSPP1ZUARAeBDJtRfdfohiswA9HxN74g"
            },
            {
                "account_id": "lavenderfive.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8pRwtD6B9nmEXChkAUoqMepSTxuYsYA1ApJCrCnD1Kbn"
            },
            {
                "account_id": "nc2.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:He7QeRuwizNEhBioYG3u4DZ8jWXyETiyNzFD3MkTjDMf"
            },
            {
                "account_id": "lionstake.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GJ8aTeqkUS5TG4GpuK5SfzLsW2f3KMCvqGJ6hywBJu4h"
            },
            {
                "account_id": "moonlet.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:DNpcdKvzabtHS9j43SpzBNXbqJtGFQrFcV4keNihnDgA"
            },
            {
                "account_id": "galactic.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:9123Ho7PrHL43PY5efdBQ5Exa9h8nwtXk8jCbdSTuZaP"
            },
            {
                "account_id": "avado.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7ytprHZpyB4QLsWakpsXkdWohsmz8VmQR9FDKhzJerNC"
            },
            {
                "account_id": "anonymous.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:42oqEsAhhgVSRDF9G2sP9FrNpUMYDStFXcYBoGzxHNMy"
            },
            {
                "account_id": "everstake.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:551hb2vAh3C4rVRD2ppZv5Q3NUVLZZx5RipTJEReyNfZ"
            },
            {
                "account_id": "01node.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Bjy4baS4MQM7FEQS4YS73boS4hJ6sdEgrfZCjqS5SXoo"
            },
            {
                "account_id": "qbit.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GAEaExXRu6pSQCnukDtaSwXspFLssxuqZgSQ3LKvwRia"
            },
            {
                "account_id": "zavodil.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6ybckHHwkwxTynYkgTn8S9mUkP39KsC8jiNqGs8i96A8"
            },
            {
                "account_id": "dokiacapital.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7DeozvoAmm2u1rVk4mbwzurh2iZGcYLDEfAMg51a8HX9"
            },
            {
                "account_id": "lux.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5dTVEqPqAsMGU82uEQCh2zNzF8Z6JNaAga5RGu77d7Fa"
            },
            {
                "account_id": "ni.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:87rLDxFERcU2JFkfgvjteCjbb6F9vrBaNdYnByArPTUu"
            },
            {
                "account_id": "future_is_near.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:31TMqceMdT1LSUAsmJbXJwnzQMvmM9LeUpJw9QMJk8xA"
            },
            {
                "account_id": "infiniteloop.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:3LzusCmBua2HHceM13LcGXvB2Du6AvK2zS8oVP32RxZM"
            },
            {
                "account_id": "bisontrails.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2VaBhZM54NukrPenMcCLwmitaKZaSPnyEhqr7mKjDvPj"
            },
            {
                "account_id": "finoa.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BqVtHqHkivBJqCnfUGpPjBFGjCfyWQfxC3K4ojdxDh17"
            },
            {
                "account_id": "abl_pool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8GexKCjsD9EfvhiRCu8RbN7PkCp37wqpLdPsvHCFjwXE"
            },
            {
                "account_id": "shardlabs.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:B7WczmEjs58xLwzspSfSbgHde3PbjTrm4me7VqhhTRss"
            },
            {
                "account_id": "republic.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:C1tyDW2eJJRZwytxDs6zC7FMPWZeBHabvjew2eZwavjo"
            },
            {
                "account_id": "electric.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GkRjmuFx61XbW7pHbsQDXvZP4Y8vavLznQLfoFLqzB2C"
            },
            {
                "account_id": "sharpdarts.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:FTxBpjgqazSoPf8cx6WNd9Cnth6eqUpBbwdKhBzYwZVM"
            },
            {
                "account_id": "anchikovproduction.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:ENsGcpMAWqgeLrGM6HApAoVSctDkMGXxuTQ8RjP1rovo"
            },
            {
                "account_id": "stakesstone.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BKgRXmMYuWXwTzS9izTh1g7NYL5q2A8azywfz9i8eUg9"
            },
            {
                "account_id": "ib.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7gtwxkU1iersMmzU8qhatwRCH4DsSPBJQSVHVN3vt1Bx"
            },
            {
                "account_id": "ideocolabventures.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:79hNcG9HreqRKWfbucFRZ8abx12uBiaehu8PrbN5AHDK"
            },
            {
                "account_id": "4ire.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5A1VMwmY9JBayxd2RocuD8mw3cib5e3JqctgEWUVFHkT"
            },
            {
                "account_id": "appload.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8hmTkSTnfZ8D3BLmr2zAXZyxrUnZwhXbp8XwpJPh1eaA"
            },
            {
                "account_id": "stake1.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:6RN8dGN2PGuwGNPL8cw5FcDLZGcGcWXnHtfefTPTAC4w"
            },
            {
                "account_id": "legends.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:71pkXGFQ3Rxw64GdH2fo6ssk9Js9EcoT6SYgGpYsJcbr"
            },
            {
                "account_id": "galaxydigital.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BVSC4oqVpa2KFhwWdiMt64ZAcizQBW23MN6RN3v56SQX"
            },
            {
                "account_id": "northernlights.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2PRvU1k6mz3XPCCXNVe2UCfRjcnsLuXbNtY6AmEBYXWo"
            },
            {
                "account_id": "n0ok.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:BiATzMX7KvWk7euGvvLLNiaVAd6LCvsqXGzU4rwCBX5N"
            },
            {
                "account_id": "guli.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:JDL27s612oXj981CfYtrs7J5JDBY5PpXLkRhmNv9QwkW"
            },
            {
                "account_id": "stakedao_retail.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Cz5wWN6fWukwtHJS7a63XfvFURd2DFNCphRRQWNZSZrS"
            },
            {
                "account_id": "chelovek_iz_naroda.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GyuMR3KYDMVQZVH87aZqHSRgqsD1ZTsRMN8JZj1gCa2P"
            },
            {
                "account_id": "projecttent.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:7uDSFrxFQ8E6YE4TdYshFjQ5FYoPHKULvFCxNzua769V"
            },
            {
                "account_id": "oraclepool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:DRsBrqty2GR6u5ELGxqJNEAbWhSzfLseiuuxWLriY6UV"
            },
            {
                "account_id": "thepassivetrust.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Gm5r656BeM4MBiQnrr9xdqVTRcFMqoYe8YygpGspyQCo"
            },
            {
                "account_id": "okexpool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:8SaYUoiXAJ6MGHi9BHPgqQrA56XrKQPk3uT1AUJPBDWN"
            },
            {
                "account_id": "aurora.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:LU8x57LmNw9MwGJoxAFAtZWgrrBRq9HnR4Y5PVjmYP9"
            },
            {
                "account_id": "tottenham_hotspur.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GG2yZ6QyxRn6mnp5BgkiHaS8jPApK2gSNfcRVY9i8UzP"
            },
            {
                "account_id": "cryptotribe.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GfykKuxE2gDiExvs2XYEkceVCjs46w7cF91oZVs97wcy"
            },
            {
                "account_id": "audit_one.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:66NWk1MwLcgHhQo3o1FiX7njevyerbcDSzhaD5LytTPs"
            },
            {
                "account_id": "near8888.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:48A9grfBpaTsHZMhEPf6jzY1dJdNRjkkx9CGYhqBsvD5"
            },
            {
                "account_id": "sweden.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:4de3Y9jD5PiyiX9szXw89XqpCDDwb1kgt829Yjp1Cy8e"
            },
            {
                "account_id": "certusone.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2NLH94qBNdkLj5ZgBjhoCY12Vc9Eq31ApTebPJPXdDbw"
            },
            {
                "account_id": "alex.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5BVKQ5zZKtEUM3AHgj6KAerTpuh3CVZHtAbmVfxLbLhc"
            },
            {
                "account_id": "trillian.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:AgNBNFK718KdnSwWDjBxcDdB2ZdQ7BQUtCTxeaH74nRP"
            },
            {
                "account_id": "majlovesreg.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:G7smyAGGAA2icWUw7WkFCBXq6ndw5UrGWvaR53PnenYn"
            },
            {
                "account_id": "huobipool.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2cYuqzQo77UC7cKsEdsLLPvVhF5zLSwV8MPfRyGZYp1d"
            },
            {
                "account_id": "artemis.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:2zccWNXUjn5GaYQCiikoSk9xR69xRvJ9uBTLFmsmQvW6"
            },
            {
                "account_id": "jubi.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:EoWKQquUjnAt1jGzeHwcoNvJdBAs98jZWpMgJ1XJVMSG"
            },
            {
                "account_id": "ashert.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5tFfDk4r5mbBtxjY1x2v4XcFnbcW6Lm8AuJvzbhcyCBS"
            },
            {
                "account_id": "dialecticstake.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:M4QceEtVE9qSQWMJWZjb3byvQBb7ce2z33Q4Dn2Uj5k"
            },
            {
                "account_id": "kukulastake1.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:GC4Gzyycxq74KGqsJcjyxq8rjgC92rQs3PCK6H1nZpuY"
            },
            {
                "account_id": "bobby.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:Txxr4whJPt59GPxjzyiME9AvLUqa5Wh3L6WejkMV9mi"
            },
            {
                "account_id": "johnsmith.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:5CzxgZniwLJBoouCUqd5NNHpLsNfDTgiyjWXpqoo6DbX"
            },
            {
                "account_id": "rocknroll.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:An4idHB2XCVkPHEHaZWTUbB8uRyHNXQeKBmoTbP2bNQ8"
            },
            {
                "account_id": "nfvalidator1.near",
                "addr": null,
                "peer_id": "ed25519:B1M3sBSZkfxobSJxkeetPxWACF7Ebr8HHvDcj3R29S85"
            },
            {
                "account_id": "nfvalidator2.near",
                "addr": null,
                "peer_id": "ed25519:58qcCKpnRkG9s6RTAn642KxBXp4HjNbduQ8BvZV7YB57"
            },
            {
                "account_id": "nfvalidator3.near",
                "addr": null,
                "peer_id": "ed25519:3pEouruMbrdrjhdcQuc7mSt8qTFqEKTNUfaUXLGWRt1D"
            },
            {
                "account_id": "nfvalidator4.near",
                "addr": null,
                "peer_id": "ed25519:DoD6sWQcZr2azztfnZPogkvrjXhZwgCgh2zcrU4xXsyL"
            },
            {
                "account_id": "stakefish.poolv1.near",
                "addr": null,
                "peer_id": "ed25519:QvPjf67yZ8w2WySej2U1LgAxdSz6LdN96GkW6j55kwZ"
            }
        ],
        "num_active_peers": 30,
        "peer_max_count": 40,
        "received_bytes_per_sec": 532041,
        "sent_bytes_per_sec": 444512
    }
}
```
