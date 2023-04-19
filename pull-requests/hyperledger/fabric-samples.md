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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1024" class=".btn">#1024</a>
            </td>
            <td>
                <b>
                    fixed test-network-k8s/scripts/test_network.sh missing 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi, 

I added ${NGINX_HTTPS_PORT} at test-network-k8s/scripts/test_network.sh and test-network-k8s/scripts/channel.sh. When I run test-network-k8s/network with setting NGINX_HTTPS_PORT=31401, I encounter bugs that fabric-ca-client still request for the port 443.

Error: POST failure of request: POST https://org0-ca.zlpt.com/register
{"id":"org0-orderer2","type":"orderer","secret":"ordererpw","affiliation":""}: Post "https://org0-ca.zlpt.com/register": dial tcp 127.0.0.1:443: connect: connection refused

Now, everything works fine.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 02:40:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    chaincode-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi,

I added a typescript implementation of private data chaincode. I tested it with the private data tutorial (https://hyperledger-fabric.readthedocs.io/en/latest/private_data_tutorial.html) and everything works fine.

I can make changes, etc., if needed.

Kind regards
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 14:32:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    chore(ci): use dedicated Fabric runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 15:16:51 +0000 UTC
    </div>
</div>

