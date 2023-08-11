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

