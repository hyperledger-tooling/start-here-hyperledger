---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1455" class=".btn">#1455</a>
            </td>
            <td>
                <b>
                    Fix Clippy lints introduced in 1.62.0 for 0-3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                Makes the same updates referenced and explained here: #1454 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 13:59:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1454" class=".btn">#1454</a>
            </td>
            <td>
                <b>
                    Fix clippy lint introduced in 1.62.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
            </td>
            <td>
                This makes several changes necessary to remove all Clippy lint warnings introduced in the 1.62.0 rust release. The two main changes are: 

1. Allowing unused lifetimes in Diesel macros. 
2. Remove unnecessary allocations made when appending to an existing string
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:40:22 +0000 UTC
    </div>
</div>

