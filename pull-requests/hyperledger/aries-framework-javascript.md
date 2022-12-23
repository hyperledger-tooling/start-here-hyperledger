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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1177" class=".btn">#1177</a>
            </td>
            <td>
                <b>
                    chore(migrations)!: connections 0.3.0 migration script and tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces changes to how connection types are handled in connection records:
- Connection types were previously stored in tags under the `connectionType` label. Connection types are now directly part of the record.
- Methods to add, update and remove types in the connection service now apply directly to the record instead of tags.
- The `connectionType` property is now pluralized to `connectionTypes` to reflect the fact that the property accepts an `Array` of connection types.
- Methods in the connection API and service have also been pluralized accordingly.
- Relevant tests have been updated to reflect changes to the connection record, API and service and have been added for the connection migration script from AFJ 0.2 to 0.3.

## Related Issues

#1155 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 14:50:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    refactor(dids): use class instances in module config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the registration of did resolvers and registrars consistent with how we do it in the credentials module by requiring class instances to be passed.

Not really a breaking change as 0.2.0 doesn't allow custom modules yet
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 07:11:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    fix(connections): use new did for each connection from reusable invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When manually accepting a connection request (either connection or did-exchange) with a reusable invitation the same keys would be used in each did response. For auto accept routing was correctly configured to create new keys for each connection. This aligns the manual flow with the auto accept flow

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 12:12:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    feat!: allow to connect with self
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was previously possible in 0.1.0, but broken in 0.2.0. This allows to connect to yourelf using connections protocols and didexchange protocol

BREAKING CHANGE: the didRecord.id was previously the did iteself. However to allow for connecting with self, where multiple did records are created for the same did, the id property is now an uuid and a separate did property is added. A migration script has been provided to update all did record's ids
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 10:57:02 +0000 UTC
    </div>
</div>

