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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3341" class=".btn">#3341</a>
            </td>
            <td>
                <b>
                    fix: fix afgo interop build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes: #3340

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 17:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    feat: CL Anoncreds Crypto services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds Crypto services

**Description:**
* Fourth PR to support CL in `af-go` [#180](https://github.com/hyperledger/aries-framework-go/issues/180)
* This PR adds high-level Crypto services to work with CL Anoncreds with help of `ursa` lib

**Summary:**
* added high-level CL crypto Issuer API
* added high-level CL crypto Prover API
* added high-level CL crypto Verifier API
* added ursa-implementations for the services
* added unit tests for issue credential flow with CL crypto
* added unit tests for present proof flow with CL crypto

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 13:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    feat: KMS storage interface redesign
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * KMS storage interface now uses a minimal interface instead of requiring a full Aries storage provider implementation (from the spi package)
* With this new approach, the consumer of an Aries KMS no longer has to let the Aries storage interface/implementation design dictate how they store KMS-related data. One notable example of this is that the choice of database name is now decided by the consumer rather than by Aries.
* To ease the transition, I added a function (NewAriesProviderWrapper) to allow a consumer to continue using an Aries storage provider implementation with a KMS if they wish. This method of injecting storage preserves the existing storage behaviour (e.g. Aries-controlled database naming).

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>

closes #3331
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 23:41:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3336" class=".btn">#3336</a>
            </td>
            <td>
                <b>
                    fix: credential manifest omit optional properties
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #3335 

**Summary:**

- `omitempty` tag for mandatory properties were removed
- optional properties (with the `omitempty` tag) of custom types were changed to pointers so they can be omitted with the `omitempty` tag
- additional validation checks which were missing and more unit tests


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 13:40:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3334" class=".btn">#3334</a>
            </td>
            <td>
                <b>
                    test/support ability in AFGO to create and parse vc and vp in JWT format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>


**Title:**
Support ability in AFGO to create and parse vc and vp in JWT format

**Description:**
Added BDD tests with creating and verifying VC and VP in JWT format.
Solves: https://github.com/hyperledger/aries-framework-go/issues/3314

**Summary:**
Algorithms included:
- Ed25519
- ECDSA secp256r1
- ECDSA secp384r1



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 13:07:15 +0000 UTC
    </div>
</div>

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

