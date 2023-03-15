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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    fix: connection id in sessions for new connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a message for a connection request (either for DID Exchange or Connection protocol) is received, a session is created without any connection id associated to it (as it is not created yet).

If the party requesting a connection does not have a public endpoint (e.g. a edge agent connecting to a mediator) and the responder does not have `autoAcceptConnections` enabled, it will not associate this session to the newly created connection, forcing any call to `agent.connections.acceptRequest` to queue the messages, even if the transport used allows a persistent connection (typical case for WebSockets).

So here what we do is simply to associate the connection to the session as soon as it is created. At the moment I don't see any drawback of this strategy but will be happy to hear any situation where this could represent a problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 23:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1382" class=".btn">#1382</a>
            </td>
            <td>
                <b>
                    chore: fix example usage of indy-sdk-react-native package to show correct usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just cosmetic fix. But can be misleading, so best to fix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 18:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1381" class=".btn">#1381</a>
            </td>
            <td>
                <b>
                    feat: basic message pthid/thid support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is something we are using to keep track of the actual id of messages related to `BasicMessageRecord` and to provide a way to relate a message to another (or another ones), giving the possibility of doing a sort of `message reply` without actually defining a new protocol but using an intrinsic feature of DIDComm messaging.

I'd like to refactor `basic-messages` module to align with others (such as `proofs` and `discover-features`) and to make it adaptable to V2 protocol, but didn't want to introduce more breaking changes before releasing 0.4.0, so I simply added `parentThreadId` as an optional parameter for now.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 15:18:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1378" class=".btn">#1378</a>
            </td>
            <td>
                <b>
                    fix: remove named capture groups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                named capture groups are only supported in more recent versions of hermes

It was of course stupid from me to assume regexes would be fully supported by hermes 🙃 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-11 14:16:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    feat(askar): import/export wallet support for SQLite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for wallet export and import by copying sqlite file and executing a key rotation to the one specified in the `WalletExportImportConfig` object. Similarly, when importing the wallet it will copy the origin file to the expected directory according to wallet id and do a rekey to the key specified.

In addition, there are a few tweaks and fixes for things I found during testing such as: 

- Key object handles clearing in pack/unpack and key creation/signing/verification methods
- Check wallet database file is created before (not sure why, but Askar is not throwing Duplicate error in `Store.provision` when wallet exists). This only works for SQLite but it's better than nothing
- Use key derivation based in argon2 Int if nothing specified, as it's the default in Indy SDK AFAIK
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 22:23:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1375" class=".btn">#1375</a>
            </td>
            <td>
                <b>
                    test: increase timeout to 120 seconds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Github action runners are slow as fuck, so I've just increased them all to 2 minutes now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 13:04:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1374" class=".btn">#1374</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): use legacy prover did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `useLegacyProverDid` flag for credential request creation, which is always set when dealing with legacy indy identifiers. Some checks were added in `LegacyIndyCredentialFormatService` to make sure we are using legacy ones.

When using IndySdk, only legacy prover_did can be used, while in AnonCredsRs through this flag we can select between prover_did and entropy, unless we are using new identifiers where only entropy can be generated.

This currently makes break a test in anoncreds-rs package because it seems that, in the underlying library, entropy is required even if passing legacy identifiers.

Depends on a fix for entropy handling in `anoncreds-rs` (to be released in v0.1.0-dev10)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 12:41:08 +0000 UTC
    </div>
</div>

