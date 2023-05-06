---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    fix(js): scan fetch record limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an unnecessary chunk variable (inherited from previous Indy SDK implementation in AFJ) that is preventing `fetchAll` to retrieve all records when they are more than PAGE_SIZE. As a result, a given Scan cannot return more than 32 entries.

Simply checking for `listHandle` (`scanNext` return value) validity seems to be enough to determine if there are no more matching records.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 18:22:31 +0000 UTC
    </div>
</div>

