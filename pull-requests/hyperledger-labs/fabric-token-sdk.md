---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    updated FSC dep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-27 05:20:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    simpler token transaction flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The goal of this PR is to remove the need to distributed the fabric envelope to the participant nodes of a transaction.
It is enough that each node receives the token request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 14:04:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/583" class=".btn">#583</a>
            </td>
            <td>
                <b>
                    shared wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR adds to core/common owner wallets for long-term and anonymous owner wallets. Any driver can reuse/extend these wallets as it fits.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 08:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Delete tokens: move nilcheck and simplify the call used by HTLC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the nilcheck to make sure it gets used (Delete does not fail if the token doesn't exist).

When running two replicas of Token SDK, one instance will delete the token from the database and notify its mailman. A current limitation is that the mailman of the second replica will not be notified (if tok turns out to be nil we don't post the event). This is not new in this PR, but we should consider it when working on the statelessness of the Token SDK instance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 14:15:20 +0000 UTC
    </div>
</div>

