---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3119" class=".btn">#3119</a>
            </td>
            <td>
                <b>
                    feat: correlating invitation with propose credential message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - WACI way of using invitation as parent threadID may not work with
DIDCommV1 where parent thread ID gets reset by messenger while sending
propose credential message
- As a work around, invitation ID can be explicitly used while sending
propose credential message
- Part of #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 19:32:53 +0000 UTC
    </div>
</div>

