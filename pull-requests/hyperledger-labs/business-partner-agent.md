---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    Fix returned credential exchange id 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">load-test</span>
            </td>
            <td>
                The response of issuing(send) a credential to a holder is the credential exchange id, but the returned id is not the UUID which is needed to refer to the appropriate credential exchange.

Usage:
- this is needed to automate revocation in the load test scenario (jmeter)

Signed-off-by: Driton Goxhufi <driton.goxhufi@bosch.io>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/847"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 12:54:58 +0000 UTC
    </div>
</div>

