---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4932" class=".btn">#4932</a>
            </td>
            <td>
                <b>
                    Added a check to make sure that chaincode is actually running.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found that sometimes chaincode won't start. It waits for "Ready" message, but another message comes to it, for example "Init".
This happens when another transaction arrives during chaincode start. And it falls between the two events:
- Handler for chaincode is already there - the start process has started
- "Ready" state has not yet occurred.

I corrected the situation by checking the Handler state as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 22:02:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4931" class=".btn">#4931</a>
            </td>
            <td>
                <b>
                    Update SDK documentation links for Fabric v3 (backport #4929)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove unsupported / deprecated client application SDKs for v2.2 and earlier.
- Remove Python SDK since it targets Fabric v1.4 and does not support BFT.
<hr>This is an automatic backport of pull request #4929 done by [Mergify](https://mergify.com).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 17:32:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4929" class=".btn">#4929</a>
            </td>
            <td>
                <b>
                    Update SDK documentation links for Fabric v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove unsupported / deprecated client application SDKs for v2.2 and earlier.
- Remove Python SDK since it targets Fabric v1.4 and does not support BFT.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 08:43:15 +0000 UTC
    </div>
</div>

