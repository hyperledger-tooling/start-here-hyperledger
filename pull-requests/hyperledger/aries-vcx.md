---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/535" class=".btn">#535</a>
            </td>
            <td>
                <b>
                    AFJ Interop: Inline value of recipient keys in ddo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">interop</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 17:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/534" class=".btn">#534</a>
            </td>
            <td>
                <b>
                    Refactoring/separate handshake reuse
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 12:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    Release 0.39.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 10:21:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    Add verification to ConnectionResponse processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - ConnectionResponse defines [signer](https://github.com/hyperledger/aries-rfcs/blob/main/features/0160-connection-protocol/README.md#2-connection-response) field, which should contain the key used for signing
- The code generally assumes that the connection~sig is using verkey of the counterparty used for communication, so the signature and signer is already verified on line 122. So this is just additional verification to check the signer value is alligned with the actual signing key.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 10:16:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    AFJ interop: change format of 'id' value in public_key portion of DDO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">interop</span>
            </td>
            <td>
                # Changes:
- AFJ Interop effort: Set value of `id` attribute on `publicKey` object in format `<ddo_id>#<key_id>` instead of `<key_id>`
Eg what previously was

```
{
	"@context": "https://w3id.org/did/v1",
	"publicKey": [
	  {
	    "id": "1",
	    "controller": "S3GarpQp2ec7xh22mEvtUr",
	    "type": "Ed25519VerificationKey2018",
	    "publicKeyBase58": "EeY5R8rDJxaCoAM1ttFrCJpWCmckJqHq6CGcEjgMbb5u"
	  }
	]
}
```

Now is
```
{
	"@context": "https://w3id.org/did/v1",
	"publicKey": [
	  {
	    "id": "S3GarpQp2ec7xh22mEvtUr#1",
	    "controller": "S3GarpQp2ec7xh22mEvtUr",
	    "type": "Ed25519VerificationKey2018",
	    "publicKeyBase58": "EeY5R8rDJxaCoAM1ttFrCJpWCmckJqHq6CGcEjgMbb5u"
	  }
	]
}
```


Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 09:03:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    Extract out trust_ping, discovery, oob protocol out of connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                - Previously, connection protocol state machine contained handling for trustping protocol. This doesn't make sense, because trustping is its own protocol and after connection is completed, trustping messages do not ever change state of connection itself.
- With this PR, trustping is extracted out and is worked with on `Connection` handler level. This makes sense, because for trustping to happen, we only need to know the DDO of the counterparty - whether we are on invitee or inviter is irrelevant (more cases like this exist).
- Changes are done in a way to improve `aries-vcx` API, but keeps `libvcx` same and backwards compatible 
- On aries-vcx Connection handler level, we now distinguish 2 public functions 
  - `update_state_with_message` - this is meant to progress the connection state
  - `answer_message` (new) - this is meant to easily-answerable messages which do not progress connection state, such as if we receive `ping`, we can send response.
- Overally this separates concerns, decreases duplication, improves composability

Analogous changes will be done for `hadshake-reuse` and `handshake-reuse-accepted`, `query ` and `disclose`.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-31 17:21:24 +0000 UTC
    </div>
</div>

