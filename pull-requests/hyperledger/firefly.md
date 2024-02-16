---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1468" class=".btn">#1468</a>
            </td>
            <td>
                <b>
                    Add map example to Tezos docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 21:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1467" class=".btn">#1467</a>
            </td>
            <td>
                <b>
                    fix: Status call returns properly when node is not registered but organisation is
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ref: https://github.com/hyperledger/firefly/issues/1453 and [this change](https://github.com/hyperledger/firefly/commit/4696ad1c82194580c3c8bf01632c020db86a74e7#diff-e097a0bac30f72e5cc6978dc4e6336e1377310f01235622293baf87758df9302R111)

When a namespace is registered to the organisation but the node has not been registered, if the name has not been set (i.e. it's `""`) then we throw an error. If a name _is_ set, then we return `nil` because while there is no information on the node (as it's not registered) it is possible for the node to be registered.

Side note: getting an environment in which to test this was a colossal pain and largely undocumented, so I'm going to put a comment below with how I got a testing configuration in place to test this out.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 11:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1464" class=".btn">#1464</a>
            </td>
            <td>
                <b>
                    Add Tezos connector to README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-10 15:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1463" class=".btn">#1463</a>
            </td>
            <td>
                <b>
                    Intermittent unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pr fixes for #1428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-10 13:50:58 +0000 UTC
    </div>
</div>

