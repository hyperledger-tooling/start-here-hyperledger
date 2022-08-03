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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/526" class=".btn">#526</a>
            </td>
            <td>
                <b>
                    Release 0.38.0
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
        Created At 2022-07-27 18:15:47 +0000 UTC
    </div>
</div>

