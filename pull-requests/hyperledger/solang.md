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
                PR <a href="https://github.com/hyperledger/solang/pull/1599" class=".btn">#1599</a>
            </td>
            <td>
                <b>
                    LLD: Clean up context after linking each contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The LLD entry points are not safe to re-enter without destroying their state. Coincidentally this worked so far but will break apart for example when compiling multiple contracts in `RelocMode::PIC`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 19:23:10 +0000 UTC
    </div>
</div>

