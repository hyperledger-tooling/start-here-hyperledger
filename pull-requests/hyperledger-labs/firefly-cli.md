---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Do not deploy Payment contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is no longer used. It will be superceded by the new work on Tokens
when available.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 16:14:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Check HTTP status code for contract deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This also revealed that it's not necessary to separately call
RegisterContract if DeployContract was already called on the node with
registeredName (it returns 409 since the contract was already registered).

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 20:58:11 +0000 UTC
    </div>
</div>

