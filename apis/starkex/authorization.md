

# Authorization
Authorization for all requests is done by providing bearer token as a value to **Authorisation** header

Authorization to all private calls can be achieved by providing nonce with the signed using an Ethereum private key message.
The value used in **GFM-StarkEx-Authorization** header gives access to private actions

#### **Example**

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
let objJsonB64 = Buffer.from(AuthHeaderbase64).toString("base64");

console.log("EcRecover", objJsonB64);

```

Result

```javascript
EcRecover eyJub25jZSI6InYyLTE2NDM4MTQwMTMuNTY3Iiwic2lnbmF0dXJlIjoiMHgyNjUxNzIzMGJlMTNjZmUzNTQ0NDdiZjMwOWEyMTZhYzQ1Y2E1ODNhOGMyNmU3NDcyNWNjY2MzNmFkZjI0OGYwMjE0MTAzZTI1MjM2MDY0ZDQxNWNhZWVlZTBhNjk2ODgzNWZiNTFhN2JiNTBhNTcyZmQxNTlmNDRiMDcwZGJkNDFjIn0=
```