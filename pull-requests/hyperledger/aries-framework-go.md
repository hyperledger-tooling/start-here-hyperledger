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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3343" class=".btn">#3343</a>
            </td>
            <td>
                <b>
                    feat: CL Anoncreds Remote KMS/Crypto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds Remote KMS/Crypto

**Description:**
* Fifth PR to support CL in `af-go` [#180](https://github.com/hyperledger/aries-framework-go/issues/180)
* This PR implements/supports CL methods in remote Crypto
* This PR adds support for KMS extension for remote KMS 
* "server"-side changes will be implemented in the separate PR in both `trustbloc/kms`

**Summary:**
* added client calls to CL methods in remote crypto
* added attrs propagation for remote kms
* added unit tests for remote kms/crypto
* added more failed cases for localkms ursa tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 13:53:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3342" class=".btn">#3342</a>
            </td>
            <td>
                <b>
                    refactor: A few refactoring of legacy-connection package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Refactor legacy-connection package due to interoperability issues

**Summary:**

- Add new legacy http header to handle legacy requests. Cover with unit tests
- Encode invitation Recipient key to base58
- Change embedded verification to referenced while creating verification methods
- Add legacy file into doc package to convert DIDdoc to raw doc. Cover with unit test
- Add handling DID id's where did method is not specified
- Add JSONBytes and ParseConnection methods to use them while handling connection data
- Change AckMsgType content to proper one
- Add method to convert array of did-keys to base58 keys
- Enable saving decryption key while handling envelope at connection-request state
- Add new InvitationRecipientKeys into connection.Record model
- Refactor requestMsgRecord, handleInboundRequest and prepareConnectionSignature methods and their unit-tests
- Save Recipient keys while handling connection request
- Use SaveDID instead SaveDIDByResolving


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 14:31:16 +0000 UTC
    </div>
</div>

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
* To ease the transition, I added a function (NewAriesProviderWrapper) to allow a consumer to continue using an Aries storage provider implementation with a KMS if they wish.
* When using Local KMS before, "k" was prepended to all keyset IDs being stored. This was a workaround for CouchDB, which would fail if someone tried storing a key using a keyset ID starting with "_". This prefixing was removed as part of the overall new philosophy of removing database-specific logic from Aries and letting the caller control their database design. Existing Aries implementations will need their databases updated to remove the "k" or, if using CouchDB and keyset IDs beginning with "_", then keyset IDs will need to be prefixed outside of Aries before trying to store/retrieve/delete from a KMS store.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>

closes #3331
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 23:41:15 +0000 UTC
    </div>
</div>

