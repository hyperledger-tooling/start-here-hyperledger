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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/847" class=".btn">#847</a>
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
        Created At 2024-07-06 08:26:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    Increase timeout for restarting agents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increased the timeout for restarting agents mid feature run. This happens in the DIDTransport tests. This is an attempt to fix the failures in the ACA-Py and AFJ runset where sometimes running in the context of the interop test pipeline most tests will fail. It looks as if at some point in the DIDTransport tests the acapy agent either fails to start or the test is not waiting long enough for it to be started and make the `status` api call then continue the tests. This increases the wait time to check the status to see if it is just ACA-py taking a little more time to startup in that environment. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 20:10:56 +0000 UTC
    </div>
</div>

