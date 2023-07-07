---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Fix escaping in LIKE expressions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Explicitly specify '[' as the escape character in all cases, and use it to escape the wildcards '%' and '_' in LIKE expressions. Works for Postgres and SQLite.

Fixes #83
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 16:23:07 +0000 UTC
    </div>
</div>

