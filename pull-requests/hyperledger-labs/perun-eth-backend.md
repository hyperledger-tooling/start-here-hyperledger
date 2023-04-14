---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    Go-Ethereum 1.11.3 compatibility (no version bump)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go-Ethereum 1.11.3 changes how `BlockChain.CurrentBlock()` works: Instead of returning a `*types.Block` it returns a `*types.Header`. This commit changes it to use `BlockChain.CurrentHeader()`, which is sufficient for us and will not break when bumping Go-Ethereum to version 1.11.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 11:49:42 +0000 UTC
    </div>
</div>

