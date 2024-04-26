---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    Adjust DID prefix check on responder call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR lightens a check that expected a specific type of Peer DID on the their_did property in the Responders response from a did-exchange/accept-request. For ACA-Py If the request is sent with a specific peer did method then the DIDs in this response with have that prefix. However I'm not checking that complete prefix here in case there are other frameworks that behave differently in this case. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 16:11:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 03:19:04 +0000 UTC
    </div>
</div>

