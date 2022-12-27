---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    chore(migrations): add generated test 0.2 connection records for migration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a follow up to #1177 and includes generated test connection records from [this script](https://github.com/petridishdev/aries-framework-javascript-test-data-generator/blob/main/index.ts) along with migration tests and snapshots for AFJ update from 0.2 to 0.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 21:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    fix: missing migration script and exports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unfortunately, `migrateDidRecordToV0_3` was not added to `updateV0_2ToV0_3` script, meaning that DID records were not upgraded, making DIDs non-resolvable.

This PR fixes that and also exposes a few classes that are mentioned in [the documentation](https://aries.js.org/guides/updating/update-assistant) but were no exported directly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 17:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    feat: adding trust ping events and trust ping command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kim Ebert <kim@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 21:17:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1180" class=".btn">#1180</a>
            </td>
            <td>
                <b>
                    refactor(wallet)!: remove wallet.createDid method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes the `wallet.createDid()` method from the agent. The did registrar module should be used instead to create indy dids. 

The agent.publicDid is kept in for now as it is needed by the ledger module, and we need it to add the endorser did to the agent. Intend to add a feature soon to add an existing did to the agent (for endorsement)

Also adds `@deprecated` tags to all wallet / agent public did functionality that is left to indicate these are deprecated and will be removed once we have replaced the ledger module (which will be when the new anoncreds module is ready). 

I think this is a big step in making AFJ not Indy focused.

There's some gaps in the dids module we need to resolve before it can be fully replaced, mainly:
- Migrate public dids created with the wallet to did records (can be done using a migration script I think)
- Allow to store a created did without necesarily writing it to the ledger. This is the case with endorser dids, where I add the did based on a seed, and the did is already registered on the ledger. I think a method like `storeCreatedDid` where you pass the did, it will resolve it to get the did document with recipientKeys and you'll then be able to use it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 04:04:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    refactor: jsonld credential format improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some small improvements to the jsonld credential format services of things I discovered when using the service. It mostly includes:
- check the whole credential instead of the credentialSubject against the request
- check the created property against the proof (if it was defined)
- do not require a class as input for the credential detail options in the credentials api
- fix incorrect interfaces
- remove redundant checks 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 08:29:26 +0000 UTC
    </div>
</div>

