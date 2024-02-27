---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Add an experimental command for importing and exporting collections of contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Often a contract is meaningful only in the context of other contracts. For example, an asset issuer contract object may depend upon an asset type contract object. The type object is necessary to establish trust in the scope of the asset being issued.

In order to simplify sharing, a contract collection file packages information about a collection of contracts and their relationship to each other into a single bundle. The file that is created includes a context file that describes the relationships between the contracts and a list of contract description files that can be used to operate on the contract objects.

Note: collection operations are marked as experimental. Any use will generate a warning message when logging is turned on.

Details of the proposed functionality are found in Issue #471.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 01:15:00 +0000 UTC
    </div>
</div>

