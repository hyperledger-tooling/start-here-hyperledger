---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2456" class=".btn">#2456</a>
            </td>
            <td>
                <b>
                    Update Python image version to 3.9.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Reduces the number of vulnerabilities in the image.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 12:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2454" class=".btn">#2454</a>
            </td>
            <td>
                <b>
                    0.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 15:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 12:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2451" class=".btn">#2451</a>
            </td>
            <td>
                <b>
                    chore: relax connections filter DID format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relax the connection filter on `my_did`, `their_did` and `their_public_did` fields of the `/connections` endpoints.

These values were restricted to `did:sov` and are now open to the generic DID format.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 13:16:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2450" class=".btn">#2450</a>
            </td>
            <td>
                <b>
                    fix: handle stored afgo and findy docs in corrections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should fix ACA-Py <-> AFGo interop by correcting a case where the LegacyPeerDIDResolver was not properly dereferencing the recipient keys for the DIDComm service.

Specifically, it should fix this error:

```python
2023-08-26 14:17:42,082 aries_cloudagent.connections.base_manager ERROR Failed to resolve service details while determining connection targets; skipping service
Traceback (most recent call last):
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/resolver/did_resolver.py", line 142, in dereference
    return document.dereference(parsed)
  File "/usr/local/lib/python3.9/site-packages/pydid/doc/doc.py", line 145, in dereference
    raise IDNotFoundError("ID {} not found in document".format(reference))
pydid.doc.doc.IDNotFoundError: ID did:sov:1H6d1WS29Bcfr7Bb9tZxA#1 not found in document

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/connections/base_manager.py", line 368, in resolve_connection_targets
    recips, routing = await self.verification_methods_for_service(
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/connections/base_manager.py", line 296, in verification_methods_for_service
    recipient_keys: List[VerificationMethod] = [
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/connections/base_manager.py", line 297, in <listcomp>
    await resolver.dereference_verification_method(
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/resolver/did_resolver.py", line 156, in dereference_verification_method
    dereferenced = await self.dereference(profile, did_url, document=document)
  File "/usr/local/lib/python3.9/site-packages/aries_cloudagent/resolver/did_resolver.py", line 144, in dereference
    raise ResolverError(
aries_cloudagent.resolver.base.ResolverError: Failed to dereference DID URL: ID did:sov:1H6d1WS29Bcfr7Bb9tZxA#1 not found in document
```

This PR also fixes an error where docs that didn't have a proper did url for the ID of the service (like those received from findy) are corrected before used. For example:

```json
{
  "@context": "https://w3id.org/did/v1",
  "id": "did:sov:5qXMeLdyWEQhieFUBNw5ux",
  "publicKey": [
    {
      "id": "did:sov:5qXMeLdyWEQhieFUBNw5ux#1",
      "type": "Ed25519VerificationKey2018",
      "controller": "did:sov:5qXMeLdyWEQhieFUBNw5ux",
      "publicKeyBase58": "3dtu2WWtd5ELwRTJEPzmEJUYEp8Qq36N2QA24g9tFXK9"
    }
  ],
  "authentication": [
    {
      "type": "Ed25519SignatureAuthentication2018",
      "publicKey": "did:sov:5qXMeLdyWEQhieFUBNw5ux#1"
    }
  ],
  "service": [
    {
      "id": "did:sov:5qXMeLdyWEQhieFUBNw5ux",  // <--- Missing #some-fragment
      "type": "IndyAgent",
      "priority": null,
      "recipientKeys": [
        "3dtu2WWtd5ELwRTJEPzmEJUYEp8Qq36N2QA24g9tFXK9"
      ],
      "serviceEndpoint": "http://172.17.0.1:9031/a2a/5b6dyY6PndLaCnWxZbeEYW/5b6dyY6PndLaCnWxZbeEYW/2f6aae0c-6b04-40ff-a25e-faecaea39f83"
    }
  ]
}
```

Fixes #2449 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-26 18:48:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    0.10.0-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 21:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    fix: ignore duplicate record errors on add key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a bandaid solution to prevent routing keys from being stored for multiple DIDs. It would be nice to correct behavior of the DIDDoc class to not turn routing keys into values in the publicKey list and then claiming that the DID is the controller (with no evidence). However, given the impending replacement of this behavior with did:peer, it doesn't seem worth it to go through that effort right now.

cc @swcurran @WadeBarnes and others
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 18:20:43 +0000 UTC
    </div>
</div>

