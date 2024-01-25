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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/536" class=".btn">#536</a>
            </td>
            <td>
                <b>
                    remove parallel flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the `SerializedPersistence` struct used to add multi-thread supports to sql drivers that do not support that. It will be responsibility of the application to use a proper driver with multi-thread support.
The PR allows the user to specify the maximum number of connections the sql db should support.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 11:53:08 +0000 UTC
    </div>
</div>

