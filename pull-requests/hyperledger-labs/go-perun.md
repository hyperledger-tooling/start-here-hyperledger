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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    wallet.CloneAddress(es)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - wallet: Add CloneAddress(es)
- channel: Use CloneAddresses in Params.Clone

It is convenient for users of the go-perun lib to have means for `wallet.Address` cloning. It was already done in `Params.Clone` so I extracted the functionality into the `wallet` package. No interfaces etc changed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 09:58:02 +0000 UTC
    </div>
</div>

