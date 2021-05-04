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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1140" class=".btn">#1140</a>
            </td>
            <td>
                <b>
                    fix: add missing connection_id to issue v2 schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @sklump, re #1135, I modified the base class which is used for both `credential_exchange_send` and `credential_exchange_create`. My bad. I created a separate schema for `credential_exchange_send` now. 

AFAIK `credential_exchange_send` should take a connection id as input (so does the code also suggest). Otherwise I fail to see the difference between `credential_exchange_create` and `credential_exchange_send`

It is weird because both have the description "Send holder a credential, automating entire flow", while they do different things.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 19:37:18 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    Add check after cred def created in integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Adds small delay plus check that cred def was created (to address random failure of integration tests)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 15:43:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    feat: feedback from responder methods about message delivery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a result of some discussion in #950, I did a quick investigation of what it would look like to provide some feedback to the responder send methods about message delivery so that from the `forward` message handler, for example, we could determine whether the message was sent directly or not. This doesn't provide a ton of information but I think it provides just enough to know whether a push notification should be sent to a mobile device or not from the forward message handler, as @TimoGlastra described in the comments of that issue.

I think there are a lot of ways to end up at similar functionality though this one ended up being simpler than I anticipated. Interested to hear thoughts.

Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 14:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1129" class=".btn">#1129</a>
            </td>
            <td>
                <b>
                    fix: do not require indy or bbs to be installed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

This should fix the issues with not having the indy and bbs libraries installed. There were a few offenders besides me for the indy library, but they should all be fixed now.

Fixes #1127
Fixes #1128 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 07:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1125" class=".btn">#1125</a>
            </td>
            <td>
                <b>
                    DIF Presentation Exchange and present-proof-v2 Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 16:48:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    Fix: stateless record webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should hopefully address #1123.

### Changes
**fix: stateless records emit events**

Error on the side of caution for BaseRecord.emit_event, using topic
without state when none is given, and inserting the serialized record as
the payload if no payload is given.

Events are only not emitted by records when no record topic is set.

**fix: relax admin server record event pattern**

Should now accept stateless record event topics

**fix: add event namespace to base records to allow plugins to override**

**test: record topic parsing for webhook**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 13:08:27 +0000 UTC
    </div>
</div>

