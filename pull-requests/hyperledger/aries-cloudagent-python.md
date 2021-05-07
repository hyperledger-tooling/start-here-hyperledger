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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1160" class=".btn">#1160</a>
            </td>
            <td>
                <b>
                    allow other service/endpoint types in indy did docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ability for the native indy resolver to get additional services / endpoint types from an indy ledger.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 17:01:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1155" class=".btn">#1155</a>
            </td>
            <td>
                <b>
                    Issue cred v2 schema fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Continuing on Timo Glastra's work: https://github.com/hyperledger/aries-cloudagent-python/pull/1140
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 16:37:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1154" class=".btn">#1154</a>
            </td>
            <td>
                <b>
                    Fix/type in ld proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Fix issue described in [Rocket chat ](https://chat.hyperledger.org/channel/aries-cloudagent-python?msg=CDike9uCQciDRohRu)
* Allow `type` property in proof validation schema
* Set default proof type if property is not provided

Currently only `Ed25519Signature2018` is allowed anyways...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 16:24:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1153" class=".btn">#1153</a>
            </td>
            <td>
                <b>
                    Tone down the endorser validation when setting up connection metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

@esune 

Removes some of the validation when setting up connection meta-data to remove timing dependencies between the author and endorser setup tasks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 14:32:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1151" class=".btn">#1151</a>
            </td>
            <td>
                <b>
                    fix: bad service endpoint in test data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>

A recent update to PyDID brought some bad input data to light.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 13:35:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1150" class=".btn">#1150</a>
            </td>
            <td>
                <b>
                    docs: update openapi file, enable multitenancy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the openapi file and enable the multitenancy api in `generate-open-api-script`

Fixes #1034 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 12:56:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1148" class=".btn">#1148</a>
            </td>
            <td>
                <b>
                    feat: send webhooks for forward messages 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds an option to ACA-Py to send webhook events on received forward messages (`--monitor-forward`, taken from `monitor-ping`).

I extended the `OutboundSendStatus` work from Daniel and added a few more status options. These are then included in the webhook event, so the controller can react to the event. 

If `--monitor-forward` is not enabled, the event is still dispatched in the event bus (just not as webhook), so other parts of the codebase/plugins can hook into this if they want to manage it in ACA-Py instead of the controller
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 12:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1145" class=".btn">#1145</a>
            </td>
            <td>
                <b>
                    Adopt problem report oob and coord mediation protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Question: what in the OOB protocol ever creates such a problem report?

In any case, this update roughs in compliance with RFC35 problem reports and adopts them into the protocol for such time as operations do create them in OOB, representing move mainly laterally but slightly better.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 14:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1143" class=".btn">#1143</a>
            </td>
            <td>
                <b>
                    Feature/didweb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work in progress PR to add the did web capabilities to ACA-PY

* Native did:web resolver
* Serve did document under `/.well-known/did.json`
* Create a did document from wallet content (uses public DID and endpoint) + additional keys (e.g.) BBS+ keys can be referenced
* Connection/DID Exchange based on implicit invitation with public did:web

Multitenancy is currently not supported.
Needs cleaning and tests.
I'm not an experienced Python programmer so there might be stupid things I've done. Would be cool if someone could take a look.

Example usage:
Assumption: ACA-Py has configured a public DID, admin interface with HTTPS (e.g. via ngrok) and a BBS+ did:key 
```
POST:  /didweb​/create-from-wallet​/{did}

{
  "verification_methods": [{
"did":"did:key:zUC71v7BaQAEpNCN9wVetcqMWtWPygSuQ2t4MJ1H9654Aio3DypS8wCd253CZ29C1CiLSMmC8MrepFYvKrvdMHBatyEoQa5pffr8HMqvRR98Vb7NtEBkpN9Ld73jyeyAqYxg8Fy", "
verification_relationships": ["assertion_method"]
}]}
```

will produce:
```
{
  "@context": "https://www.w3.org/ns/did/v1",
  "id": "did:web:478eb39f6464.ngrok.io",
  "verificationMethod": [
  {
    "id": "did:web:478eb39f6464.ngrok.io#key-1",
    "type": "Ed25519VerificationKey2018",
    "controller": "did:web:478eb39f6464.ngrok.io",
    "publicKeyBase58": "DAwrZwgMwkTVHUQ8ZYAmuvzwprDmX8vFNXzFioxrWpCA"
  },
  {
     "id": "did:web:478eb39f6464.ngrok.io#key-2",
     "type": "Bls12381G2Key2020",
     "controller": "did:web:478eb39f6464.ngrok.io",
     "publicKeyBase58": 
"n5ZJWiW1TkL9jzpoig99Db9UjQ8hN4L8UuRTfEcFRqSEpNroSGoUDd5XQ2nwUuAhJ9MK5wzqSMzxNzCWC1qs51i5cEBii2ie1i9XXCWG1dyWXKr9jRyETJdmWUEHFzoodef"
}
],
"authentication": [
"did:web:478eb39f6464.ngrok.io#key-1"
],
"assertionMethod": [
"did:web:478eb39f6464.ngrok.io#key-1",
"did:web:478eb39f6464.ngrok.io#key-2"
],
"service": [
{
"id": "did:web:478eb39f6464.ngrok.io#did-communication",
"type": "did-communication",
"serviceEndpoint": "http://host.docker.internal:8000",
"recipientKeys": [
"did:web:478eb39f6464.ngrok.io#key-1"
],
"routingKeys": [],
"priority": 0
}
]
}
```

served under `https:478eb39f6464.ngrok.io/.well-known/did.json`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 08:30:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1141" class=".btn">#1141</a>
            </td>
            <td>
                <b>
                    docs: small updates to jsonld docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just some small rewording, no substantive changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 06:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1139" class=".btn">#1139</a>
            </td>
            <td>
                <b>
                    Adopt problem reports issue cred present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                and sync up problem reports to current RFC 35
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 15:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    docs: add docs on issuing jsonld credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds documentation on issuing JSON-LD credentials. Present Proof is todo and dependant on PR #1125.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 11:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Changes in Endorser Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a WIP pull request, and it covers the changes in endorser protocol for issues defined in 

1. #1031 
2. #1029 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 18:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Add "minimum viable message" base class for use in plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #1096, when writing plugins, having the flexibility to implement messages differently than the pattern followed within ACA-Py can be really significant. This PR defines a minimized base message class that is unopinionated and trivial to extend.

This PR also addresses concerns around message serialization in anticipation of changes coming with DIDComm v2 by defining `serialize` and `deserialize` methods that specify the output/input format. At present, the `AgentMessage` class only implements DIDComm v1 message structure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 02:35:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    fix: run_tests script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>

Not sure what happened (perhaps related to Ubuntu 18.04 EOL?) but `run_tests` stopped working all of a sudden. This switches image base to `python:3.6.13`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 22:50:54 +0000 UTC
    </div>
</div>

