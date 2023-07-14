---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1441" class=".btn">#1441</a>
            </td>
            <td>
                <b>
                    Fix compiler output section in solang.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The compiler output section was not desterilized correctly from the `solang.toml` file created by `solang new`. this adds a fix for this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 02:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1440" class=".btn">#1440</a>
            </td>
            <td>
                <b>
                    Bump should be hashed by last
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we hash include the bump in the `seeds` array passed to a Solana runtime call in the same order specified by developers when they are writing the contract's constructor. This is not the intended behavior, though. The bump must always be the last element in the array. This PR ensures that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 18:38:16 +0000 UTC
    </div>
</div>

