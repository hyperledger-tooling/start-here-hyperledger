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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1026" class=".btn">#1026</a>
            </td>
            <td>
                <b>
                    Add test-network org3 affiliation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The org3 affiliation is needed when registering users for org3.

Resolves https://github.com/hyperledger/fabric/issues/4155
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 21:47:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1025" class=".btn">#1025</a>
            </td>
            <td>
                <b>
                    Fix erc-1155 sample README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instructions to setup the environment aren't quite right. This fixes it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 12:32:51 +0000 UTC
    </div>
</div>

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

