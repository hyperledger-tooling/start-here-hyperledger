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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Client tests: fail on error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Client tests involve concurrency. t.FailNow is not available there.
That's why we often used assert instead of require. Now we can use
role.Require.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 09:41:53 +0000 UTC
    </div>
</div>

