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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    refactor(proofs): createRequest for connectionless proof request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Similar approach as #772, to be able to create a legacy Out-of-Band invitation containing a Request Proof message.

Resolves #997 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 22:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1030" class=".btn">#1030</a>
            </td>
            <td>
                <b>
                    Merge branch 'main' into 0.3.0-pre
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merging 0.2.3 and 0.2.4 features into 0.3.x branch:

- All tests pass
- Demo works
- Action Menu module was added to the core for the moment

Hope to not have missed anything. Please double check!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 20:11:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1029" class=".btn">#1029</a>
            </td>
            <td>
                <b>
                    feat: use did:key flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An initial step to support [Aries RFC 0360](https://github.com/hyperledger/aries-rfcs/tree/main/features/0360-use-did-key) by adding an optional configuration flag `useDidKeyInProtocols` that will define how agent should format keys in protocols where keys are exchanged: 'naked' (base58) or did:key encoded. 

This setting will be used unless the other party has already sent us keys (for instance, a Mediator sent us the routing key in a Mediation Grant message). In such case, their format will be used in subsequent messages for that protocol (e.g. KeyList Update). This is achieved by adding a specific metadata key `UseDidKeysForProtocol` to the related connection record, which  intended to track the other party support of did:key in different RFCs. 

Currently, only Coordinate Mediation (RFC 0211) uses this feature, but in further versions other protocols will use this metadata/settings key (such as Pickup V2 - RFC 0685). 

For key reception, the agent will always accept both formats and internally store in base58.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 02:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1028" class=".btn">#1028</a>
            </td>
            <td>
                <b>
                    feat: add getRequestedCredentialsForProofRequest 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The method getRequestedCredentialsForProofRequest was present in the API before the PPV2 code was merged but somehow got lost.

It has been restored in this PR
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 06:38:28 +0000 UTC
    </div>
</div>

