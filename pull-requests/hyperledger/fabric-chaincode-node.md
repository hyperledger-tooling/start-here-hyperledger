---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Publish multi-arch, arm64 docker image - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DO NOT MERGE**

Publish a multi-arch fabric-nodeenv image with a GHA buildx builder.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 20:47:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Fix issues with server-mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - removed possible issue with stream referring to the correct value, due to difference in scoping between function() and ()=>{}
- ensured that in server mode, the promise was awaited for
- fixed the register message being sent as the wrong type
- note the addition of the delete call - for some reason this was picked up by the coverage tests which it never has been before...


Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 14:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/366" class=".btn">#366</a>
            </td>
            <td>
                <b>
                    Adding new format for getID()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: aruns05 <arun.s2k8@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 12:42:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    Update to v3.0.0-unstable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 13:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    Forward Port all Release 2.5 Changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move up the release-2.5 changes to main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 09:08:58 +0000 UTC
    </div>
</div>

