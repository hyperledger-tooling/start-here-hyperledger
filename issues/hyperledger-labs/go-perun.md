---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/go-perun/issues/280" class=".btn">280</a>
            </td>
            <td>
                <b>
                    Implement Data.Equal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                Yes, because when validating a state we use it to compare `Data` ([here](https://github.com/boschresearch/go-perun/blob/eca5f7032ad79411c06b86d8a5af9144bb954cd9/channel/state.go#L143)).

However, in a separate PR, we could implement `Data.Equal` and then remove this function.

_Originally posted by @manoranjith in https://github.com/hyperledger-labs/go-perun/pull/272#discussion_r763697134_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 09:18:07 +0000 UTC
    </div>
</div>

