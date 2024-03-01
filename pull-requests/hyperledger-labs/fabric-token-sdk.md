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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    Move msp
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
        Created At 2024-03-01 11:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    network service cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR proposes the following:
- remove transient-related function from the network service, they are not needed anymore
- cleanup sql db logs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 10:16:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/557" class=".btn">#557</a>
            </td>
            <td>
                <b>
                    `tokendb` and `tokens`'s support for transactions
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
        Created At 2024-02-28 14:57:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    golangci-lint
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
        Created At 2024-02-28 11:57:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    move owner into ttx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR moves the owner service inside the ttx service. This is in alignment with `audit` and `auditdb` services, and `tokens` and `tokendb` services.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 07:54:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/554" class=".btn">#554</a>
            </td>
            <td>
                <b>
                    tokens service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR introduces the `tokens` service used to update the `tokendb` starting from a `TokenRequest`. 
The fabric and orion processors will use this service to commit locally the transactions.

In the following PRs, we will address the following points:
- Atomicity of  `AppendTransaction`. If a failure happens, no traces should be left in the `tokendb`.
- Ability to remove all the records related to a given transaction
- Fix  the TODOs in `EndorseView`'s `receiveTransaction` function
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 09:34:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    add dependency to the hash of public params in the rws
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR adds an additional dependency to the current public parameters in the RWSet. 
This is helpful every time one wants to update the public parameters without upgrading the chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 13:38:49 +0000 UTC
    </div>
</div>

