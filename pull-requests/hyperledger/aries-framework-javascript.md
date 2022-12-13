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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1156" class=".btn">#1156</a>
            </td>
            <td>
                <b>
                    feat(oob): receive Invitation with timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 07:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1153" class=".btn">#1153</a>
            </td>
            <td>
                <b>
                    refactor(proofs): remove proofrequest property
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolves #1114 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 09:29:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1151" class=".btn">#1151</a>
            </td>
            <td>
                <b>
                    fix: expose OutOfBandEvents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Moriarty <moritz@animo.id>

closes #1150 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 14:25:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1149" class=".btn">#1149</a>
            </td>
            <td>
                <b>
                    feat!: use did:key in protocols by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed some time ago in #497, now we are having a new major release, we use did:key in protocols by default. We'll of course still accept base58-encoded keys if the other party is not yet using did:key.

BREAKING CHANGE:
`useDidKeyInProtocols` configuration parameter is now enabled by default. If your agent only interacts with modern agents (e.g. AFJ 0.2.5 and newer) this will not represent any issue. Otherwise it is safer to explicitly set it to `false`. However, keep in mind that we expect this setting to be deprecated in the future, so we encourage you to update all your agents to use did:key.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 08:12:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1148" class=".btn">#1148</a>
            </td>
            <td>
                <b>
                    feat: Corrected peer DIDs resolution (key IDs)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR corrected resolution of peer DIDs of method 0 (`did:peer:0`) and method 2 (`did:peer:2`) into DID documents, specifically resulting key IDs.
For peer DIDs of method 0 and method 2, key fragment IDs are multibase representations of public keys **without** the multibase prefix (i.e. **without** `z` prefix in case of base58 encoding).

This logic is based on:
- _Example 4_ from https://identity.foundation/peer-did-method-spec/#multi-key-creation
- examples from https://github.com/sicpa-dlab/peer-did-jvm
- tests from https://github.com/sicpa-dlab/didcomm-demo/blob/main/didcomm-demo-python/tests/test_did_resolver_peer_did.py and https://github.com/sicpa-dlab/didcomm-demo/blob/main/didcomm-demo-jvm/didcomm-demo/src/test/kotlin/org/didcommx/didcomm/demo/DIDDocResolverPeerDIDTest.kt

At the same time, this PR keeps the existing resolution logic for key DIDs (`did:key`). So for key DIDs, key fragment IDs are multibase representations of public keys including the multibase prefix (as specified at https://w3c-ccg.github.io/did-method-key/)

This PR is based on https://github.com/hyperledger/aries-framework-javascript/pull/1096 which must be merged first.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 14:13:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1147" class=".btn">#1147</a>
            </td>
            <td>
                <b>
                    fix(routing): add connection type on mediation grant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small update to the feature added in #994 to aggregate the connection type when a connection is related to a mediation grant. 

Previously, it was setting **only** `ConnectionType.Mediator`, so if the connection was previously tagged with another type, it would be lost.

Also fixes typing for `connectionType` in `ConnectionRecord` in order to be able to properly query for connections matching one or multiple types.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 02:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1146" class=".btn">#1146</a>
            </td>
            <td>
                <b>
                    fix: expose AttachmentData and DiscoverFeaturesEvents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Expose AttachmentData and Discover Features events... and some minor housekeeping to remove a few lint warnings.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 21:27:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1143" class=".btn">#1143</a>
            </td>
            <td>
                <b>
                    feat: remove keys on mediator when deleting connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the case where a mobile agent (or any agent that uses mediator) deletes a connection or OOB record, meaning that the corresponding recipient keys should be removed from its mediator (as per [Aries RFC 0211](https://github.com/hyperledger/aries-rfcs/blob/main/features/0211-route-coordination/README.md)). Otherwise, mediator will still be forwarding messages to the agent that can't (and more importantly _don't want to_) be handled.

This will mean that, when using mediator, in order to delete a connection or out-of-band record, the agent must be online. This is aligned to the opposite case: connection and OOB invitation creation, which also need the agent to be online to be in sync with its mediator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 03:11:32 +0000 UTC
    </div>
</div>

