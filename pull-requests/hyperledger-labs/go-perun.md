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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    Separate wire address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #234.

In general, this PR will ensure that `wire.Address` and `wallet.Address` are distinct. Before, `wire.Address` was a synonym for `wallet.Address`, which caused some problems, in particular, mixing up `wire.Address` and `wallet.Address` and adding functionality to `wallet.Address` which was specific to the use case of `wire.Address` (concretely, the `Cmp` function).

In this PR we assign both their own type.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 07:49:31 +0000 UTC
    </div>
</div>

