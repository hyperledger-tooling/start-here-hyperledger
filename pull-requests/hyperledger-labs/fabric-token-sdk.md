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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    add an option to stop the htlc scan for preimage when all blocks are …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …searched until the tip of the blockchain.

Can be used for a better experience if triggered by a user and you want to show them immediately whether the preimage is available on the current ledger, instead of having to wait until timing out.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 15:24:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    cleaup service provider's use in services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following:
- Use token.ServiceProvider rather than view.ServiceProvider.
- Remove ServiceProvider as a field where possible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 14:51:43 +0000 UTC
    </div>
</div>

