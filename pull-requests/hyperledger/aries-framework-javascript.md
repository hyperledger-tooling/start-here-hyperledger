---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1495" class=".btn">#1495</a>
            </td>
            <td>
                <b>
                    fix: race condition singleton records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/aries-framework-javascript/issues/968

This just handles the multiple creation and then erroring of signleton records. 

We still have an issue with multiple writes to the same document, which we should be able to fix with locks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 12:14:03 +0000 UTC
    </div>
</div>

