---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Use built-in Peer chaincode-as-a-server builder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using the variant of the peer's docker container from https://github.com/hyperledger/fabric/pull/2990  this PR adapts the K8S deployment to use this inbuilt chaincode builder.

- creates two deployments of the chaincode for each peer
- uses the builders ability to template the fields in the connection.json

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 10:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/523" class=".btn">#523</a>
            </td>
            <td>
                <b>
                    Updated logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - updated the logging for the application command; wasn't very good
- added some information to the help option. the current settings
  useful if you're not sure what you've set


FYI @jkneubuh 

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 09:29:47 +0000 UTC
    </div>
</div>

