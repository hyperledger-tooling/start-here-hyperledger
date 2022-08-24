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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3345" class=".btn">#3345</a>
            </td>
            <td>
                <b>
                    feat: wallet.Issue supports jwtvc, verifiable.Credential can hold a jwtvc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 19:13:12 +0000 UTC
    </div>
</div>

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

