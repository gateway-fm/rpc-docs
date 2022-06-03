---
description: >-
  Below you will find the api documentation for the standard Gnosis JSON-RPC
  calls that Gateway supports.
---

# Gnosis API
Gateway.fm provides public Gnosis RPC in the Asia region
so this common url https://rpc.<REGION>.gateway.fm/v1/gnosis/non-archival/mainnet 
should be substitute by
https://rpc.ap-southeast-1.gateway.fm/v1/gnosis/non-archival/mainnet

If you use public RPC you don't need authorization Bearer token,
it means that this header should be deleted from your request:
-H "Authorization: Bearer <YOUR_API_KEY>" 