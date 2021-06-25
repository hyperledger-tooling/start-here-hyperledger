---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    Improve typescript definitions in scenario steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the node scenario test driver, the currentGateway could, in theory, be undefined.  The Gateway identity should always be defined.
The typescript code has been changed to assert these are behaving as expected.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 09:08:16 +0000 UTC
    </div>
</div>

