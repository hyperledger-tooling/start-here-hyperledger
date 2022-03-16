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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Override default port of CA connection on CCP teample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Signed-off-by**: Charalarg [charalarg@gmail.com](mailto:charalarg@gmail.com)

**Type of change**:
- Bug fix

**Description**:

In test-network-k8s the certificate authorities are deployed with TLS enabled under the port 443. But the connection profile template implements a connection to the default (7054) port of the certificate authority. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 15:21:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/675" class=".btn">#675</a>
            </td>
            <td>
                <b>
                    Update nano test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix minor bugs, add network.sh script to simplify standing up the network, and add an option to run the network in a single container

Note: the updated peerNadmin.sh scripts no longer create or join a channel and now only configure the environment for the relevant peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 16:04:19 +0000 UTC
    </div>
</div>

