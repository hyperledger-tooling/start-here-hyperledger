---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Egoistic funding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This PR builds upon the changes introduced in https://github.com/hyperledger-labs/perun-eth-backend/pull/45 by extending egoistic funding to cross-chain swaps in the eth-backend.

In this update, we introduce a map for each chain, designating whether a chain is considered egoistic or not. This distinction is crucial in determining the funding order for different chains, ensuring that egoistic chains are funded last.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 09:19:01 +0000 UTC
    </div>
</div>

