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
                    Inline value of recipient keys in ddo
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
                    Extract out trust_ping protocol from connection protocol module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    DDO: Refactoring, support additional format of public_key.id value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Refactoring
- Separated DDO code to separate module
- Moved `Invitation -> DDO` conversions out of DDO next to invitation code
- Refactored DDO code, especially concerning references to `public_key` section, created type `DdoKeyReference`, modified function signatures to work with this type
- Renamed old ddo testing construction functions like `_did_doc_1` to have more descriptive names

# Features
- Added support to allow `id` in `public_key` objects to be in format `<key>#<key_id>` such as `Xnwiz15WsgFeN2CxQBuYo5#1`. Previously only format `key_id` such as `1` was allowed.

# Current DDO format support notes:
- we define `service` field as array of objects. These service objects reflect [aries specification](https://github.com/hyperledger/aries-rfcs/blob/main/features/0434-outofband/README.md#the-services-item) which is more rich than w3c specification for service [attribute on DDO](https://github.com/hyperledger/aries-rfcs/blob/main/features/0434-outofband/README.md#the-services-item)
- we, and seem that most other current Aries implementations define `publicKey` property on DDO, this is however not present in w3c specification. Arguably [`authentication` verification method](https://w3c.github.io/did-core/#did-document-properties) should be used instead and usage of `publicKey` should be dropped.

 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 16:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Use macOS 11 in CI
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
        Created At 2022-07-28 08:21:19 +0000 UTC
    </div>
</div>

