---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Make IsFinal work for real
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The way how we implement broadcasting a transaction and then waiting for it to commit is inherently flawed:

1. We send it to the orderer
2. We connect to the orderer and start listening for blocks starting from the last block.

After (1) and before (2) the transaction might already enter a block and then (2) will miss it.
Moreover, the way (2) is implemented is connecting to the peer's delivery service and it just doesn't scale well when many transactions should be sent and waited for.

Implemented a pub-sub mechanism that is piggybacking on the already existing background task that pulls blocks and parses them. 


Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 00:57:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Lock when sending
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:04:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Do not closeSend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 17:32:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    fix deadlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 17:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    FlowControlBroadcast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 16:50:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Add command to kill FSC nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 16:14:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Increase default batch size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 12:25:50 +0000 UTC
    </div>
</div>

