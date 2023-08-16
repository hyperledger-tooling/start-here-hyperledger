---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Delete mediation record if it's not ready
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a bug introduced by the previous PR #59 
We have to delete the old mediation record in both cases:
1. when the mediatorConnectionsInvite has changed
2. when the mediation status is not ready (mediation protocol started but not completed)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 08:57:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Assert the mediator invitation url is same to that of mediation record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the mediatorInvitationUrl in AgentConfig is changed, we remove the old mediation record and do the mediation protocol again.
There was a path that we omit the url check.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 07:33:55 +0000 UTC
    </div>
</div>

