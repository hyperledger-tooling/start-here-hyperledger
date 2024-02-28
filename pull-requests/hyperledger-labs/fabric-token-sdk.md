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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/551" class=".btn">#551</a>
            </td>
            <td>
                <b>
                    simplified token processor and db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR simplify the `TokenStore` interface unifying the function to append new tokens. As a byproduct, this PR also reworks the data model used by the tokendb's sql implementation. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 08:06:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/550" class=".btn">#550</a>
            </td>
            <td>
                <b>
                    identitydb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - create identity service used by the drivers
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 10:57:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    Simplify the network service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to simplify the network service to the bare minimum and avoid any reference to underlying backend concepts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 17:41:54 +0000 UTC
    </div>
</div>

