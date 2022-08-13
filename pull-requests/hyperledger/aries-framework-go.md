---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3332" class=".btn">#3332</a>
            </td>
            <td>
                <b>
                    feat: implement signer.Alg()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 19:17:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3329" class=".btn">#3329</a>
            </td>
            <td>
                <b>
                    feat: CL Anoncreds KMS extension
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds KMS extension

**Description:**
* Third PR to support CL in `af-go` [#180](https://github.com/hyperledger/aries-framework-go/issues/180)
* This PR adds support for CL CredDef and MasterSecret keys in KMS
* This PR extend KMS API methods to support extra parameters on key's creation/rotation/export
* `remotekms` and `remotecrypto` changes will be implemented in the next PR in both `af-go` and `trustbloc/kms`

**Summary:**
* extended kms API key create/rotate/export with extra options
* added CL CredDef and MasterSecret keys to localkms
* implemented CredDef pubkey export
* refactored keytemplate resolving
* added unit tests for CL keys
* re-generated kms's mock


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 15:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3328" class=".btn">#3328</a>
            </td>
            <td>
                <b>
                    fix: change validate->Validate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed credentialManifest's `validate()` back to `Validate() `as it needs to be exported
Signed-off-by: heidihan0000 <daeun.han@avast.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 14:42:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3325" class=".btn">#3325</a>
            </td>
            <td>
                <b>
                    feat: Add client, rest and command handlers for legacy-connection pro…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Add client, rest and command handlers for legacy-connection protocol

**Summary:**

- Add client for legacy-connection protocol
- Move didexchange.Event to didcomm/common/event.go in order to make it common for didexchange and legacy-connection protocols
- Refactor HandleInboundEnvelope method of inbound message handler in order to handle messages of legacy-connection protocol
- Add rest and command handlers for legacy-connection protocol. Use them inside controller package
- Add creating legacy destination
- Add new LegacyConnection Error group
- Enable handling base58 keys while packing legacy media type envelopes
- Change media type profile while initializing legacy-connection service

Closes #3300 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 07:55:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3324" class=".btn">#3324</a>
            </td>
            <td>
                <b>
                    fix: vc subject marshal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 16:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3322" class=".btn">#3322</a>
            </td>
            <td>
                <b>
                    fix: JWS algorithm for signature suite 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>

closes #1589
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 09:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3320" class=".btn">#3320</a>
            </td>
            <td>
                <b>
                    feat: allow mediator GetConnections APIs to filter by didcomm version.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #3321 

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 23:40:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3319" class=".btn">#3319</a>
            </td>
            <td>
                <b>
                    fix: presentation with empty credential fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes how a presentation is marshalled with empty credential field which wrongly outputs:
'"verifiableCredential": null'

This change skips this field if the presentation Credential field is empty

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 19:12:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3318" class=".btn">#3318</a>
            </td>
            <td>
                <b>
                    Add RemoveCredentialByName to aries js helpers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Function was available in the core but was missing from the JavaScript
wrapper.

Signed-off-by: Boran Car <boran.car@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 16:44:10 +0000 UTC
    </div>
</div>

