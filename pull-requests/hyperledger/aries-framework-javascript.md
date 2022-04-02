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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    feat: add role and method to did record tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Adds the `role` and `method` to the `DidRecord` tags. This will make it easier to integrate the did registrar module later one without needing to resave all did records.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 13:25:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    feat: delete credential from wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #602, deleting a credential can now also be deleted from the wallet. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 11:57:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    feat: add update assistant for storage migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds an `UpdateAssistant` that can help with updating AFJ storage to newer versions. If the agent is initialized with an older storage version than the framework an error is thrown and the agent can't be initialized. See the updating.md doc for examples on how to use the update assistant to update agent storage.

I've also added an autoUpdateOnStartup parameter that will auto update the agent storage on initialization. Would like to have a discussion about this during the WG call whether this is desired or what the most optimal flow would be for updating the agent.

I've added two migrations for now, we can add more once the PRs are merged:
- update the role in mediation record
- update the metadata object in the credential record to the new format

The changes are well documented in the `0.1-to-0.2` document. This currently contains only breaking storage changes, but should be updated with breaking code changes also.

A backup will be created when starting the agent, and it will be restored if the migration failed.

I spent _A LOT_ of time on testing to make sure nothing goes wrong here as that can lead to nasty situations. Every migration has extensive tests and there are also quite some tests for the e2e flow.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 10:50:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    fix: did sov service type resolving
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes behavior with the service resolution & types behavior with did:sov resolution. This additionally renames the `IndyDidResolver` to `SovDidResolver` to reduce confusion and prevent collision with the did:indy method in the future. Happy for any feedback/thoughts here.


@TimoGlastra if you could take a look at this one to ensure I didn't miss something here that'd be appreciated! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 00:20:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    feat: extension module creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Export some convenience types and classes to facilitate extension/plug-in development and add a fully-working dummy extension module in samples directory.

I'm not sure if it's the right place to put all this stuff, but I believe it could help developers to add custom protocols and wallet storage to their controllers, so it's worth for it to be somewhere :-).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:38:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    refactor: remove verkeys and did docs from connection record
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
        Created At 2022-03-29 19:52:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    fix: allow to set tags in MediationRecord constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow to optionally set tags for MediationRecord in class constructor (as it is in other records such as ConnectionRecord, ProofRecord, etc.). This is not currently used in regular flows but could be useful when mocking framework records.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 16:07:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    feat: bbs createKey, sign and verify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **MARKED AS DRAFT** because the `react-native-bbs-signatures` is not yet released and merging this will break the React Native environment if bbs-signatures are being used.

Almost every change in this PR will be reverted when support for `aries-askar` is added, as we can then do all the functionality inside the wallet instead of the AFJ level. 

- Adds bls12381g1 and bls12381g2 to `indyWallet.createKey`
- Adds bls12381g2 to `indyWallet.sign`
- Adds bls12381g2 to `indyWallet.verify`
- Store and retrieve the keyPair in the wallet via the public key
- Added tests for the indy wallet
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 09:01:01 +0000 UTC
    </div>
</div>

