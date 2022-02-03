# Authorization
Authorization for all requests is done by providing Bearer token as a value to **Authorisation** header. You can obtain it from the Gateway.fm admin dashboard.

Some methods require authorisation with extra header. It could be done by providing nonce and signed message using an Ethereum private key.
The value used in **GFM-StarkEx-Authorization** header gives access to private actions

#### **Example**


EcRecover_value requires ETH private key in order to generate GFM-StarkEx-Authorization header value:
```bash
var Web3 = require('web3');
var web3 = new Web3();

const private_key = <YOUR_ETH_PRIVATE_KEY>

// generate nonce
const nonce = Date.now() / 1000
const formattedUTCDate = new Date(nonce * 1000).toUTCString()

// sign the signing in message with eth private key
const auth_message = `Signing in to DeversiFi on ${formattedUTCDate}. For your safety, only sign this message on DeversiFi.`.toString(16)
const signature = web3.eth.accounts.sign(auth_message, private_key).signature;

// Base64 encode above to use with EcRecover 
const l2_auth_header = {
    nonce: `v2-${nonce.toString()}`,
    signature: `${signature}`,
   }
let AuthHeaderbase64 = JSON.stringify(l2_auth_header)
let objJsonBase64 = Buffer.from(AuthHeaderbase64).toString("base64");

console.log("EcRecover", objJsonBase64);
```

Result

```javascript
EcRecover eyJub25jZSI6InYyLTE2NDM4MTQwMTMuNTY3Iiwic2lnbmF0dXJlIjoiMHgyNjUxNzIzMGJlMTNjZmUzNTQ0NDdiZjMwOWEyMTZhYzQ1Y2E1ODNhOGMyNmU3NDcyNWNjY2MzNmFkZjI0OGYwMjE0MTAzZTI1MjM2MDY0ZDQxNWNhZWVlZTBhNjk2ODgzNWZiNTFhN2JiNTBhNTcyZmQxNTlmNDRiMDcwZGJkNDFjIn0=
```

And with the Bearer token taken from Gateway.fm admin dashboard the next authenticated endpoint used to retrieve user balance could be requested:

```bash
curl https://rpc.gateway.fm/v1/starkex/stg/trading/r/getBalance \
-X POST \
-H "Authorization: Bearer <YOUR_API_KEY>" \
-H "GFM-StarkEx-Authorization: EcRecover eyJub25jZSI6InYyLTE2NDM4MTQwMTMuNTY3Iiwic2lnbmF0dXJlIjoiMHgyNjUxNzIzMGJlMTNjZmUzNTQ0NDdiZjMwOWEyMTZhYzQ1Y2E1ODNhOGMyNmU3NDcyNWNjY2MzNmFkZjI0OGYwMjE0MTAzZTI1MjM2MDY0ZDQxNWNhZWVlZTBhNjk2ODgzNWZiNTFhN2JiNTBhNTcyZmQxNTlmNDRiMDcwZGJkNDFjIn0=" \
-H "Accept: application/json" \
-H "Content-Type: application/json" \
-d '{"token":"ETH"}'
````
