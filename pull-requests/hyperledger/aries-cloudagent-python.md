---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2086" class=".btn">#2086</a>
            </td>
            <td>
                <b>
                    fix: create local DID return schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a follow-up to the changes in the creation endpoint (#2067), relax return schema to include any did method.

Without this change, clients based on the openapi spec cannot accept the response payload for did methods other than "sov" and "key".

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 08:19:22 +0000 UTC
    </div>
</div>

