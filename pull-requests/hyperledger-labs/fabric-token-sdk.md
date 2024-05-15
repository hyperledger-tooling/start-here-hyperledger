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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    revert changes: compute max value using big int
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Putting back Arne's code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 14:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    identity deserialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following:
- It introduces an alias of `view.Identity` from the smart client in the Token and Driver API. In future PR, the alias will be used everywhere and then the dependency to the smart client removed.
- It refactors the identity deserialization infrastructure to be more customizable. The identity type tells which deserializer to use in all circumstances.

Side node: This PR leaves a TODO to be addressed in another PR. The auditor of the zkatdlog driver needs to be updated to better handle the htlc identities and their relative audit information.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 05:28:09 +0000 UTC
    </div>
</div>

