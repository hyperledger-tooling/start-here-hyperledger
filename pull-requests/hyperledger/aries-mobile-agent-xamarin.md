---
layout: default
title: aries-mobile-agent-xamarin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-xamarin
---

# aries-mobile-agent-xamarin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-xamarin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-xamarin/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Fix connection issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the following issues:
1) Stuck in Negotiating state when other agent accept the invitation created (QRCode) on the mobile agent. Fix: Add AutoAcceptConnection = true
2) No label in the invitation created on the mobile agent. Fix: Add invitation.label
3) Other agent unable to read the invitation message because it does not recognise d_m tag.  Fix: change to c_i tag (RFC 0160)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 10:17:20 +0000 UTC
    </div>
</div>

