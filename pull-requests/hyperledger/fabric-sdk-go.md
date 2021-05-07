---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Discovery selection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Do not ignore peers, which were received from DS(DiscoveryService), but are not specified in EndpointConfig. A single org can't possibly know about all existing peers in the network, so it's enough to define at least one, which will be entry point to the DS. Added/fixed tests.
Related issue: https://stackoverflow.com/questions/67044235/fabric-invoke-chaincode-error-failed-to-get-endorsing-peers-no-endorsement-com/67437604#67437604
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 17:12:00 +0000 UTC
    </div>
</div>

