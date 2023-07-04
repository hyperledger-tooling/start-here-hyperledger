---
layout: default
title: harmonia
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/harmonia
---

# harmonia <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/harmonia){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    Recursion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes the `put`, `get`, `generateMerkleProof` and `verifyMerkleProof` functions fully recursive, and delegates the implementation to each node type's class, removing a lot of pattern-matching code. It also adds some inline comments around some of the nastier details of updating the trie, and missing copyright notices on some file headers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 13:33:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Test proof of inclusion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added test that proves event was generated from a transaction that was actually included in a block.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 12:13:32 +0000 UTC
    </div>
</div>

