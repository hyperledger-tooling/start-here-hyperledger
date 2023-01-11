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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    Backport merge from release-2.5 to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR cherry-picks commits from release-2.5 to main: 

- 30125f689a872073a2c37d6c64cd683b04acd754 (Build multi-arch / arm64 hyperledger/fabric-nodeenv) 
- b35dee8d9eb574649889c02c96775c5781a7c1d2 (Pin grpc-js to 1.8.1) 
- 0bd21b79bab7b3e5b89f8f0c908b4e6f7aed72f4 (Update to use arrow functions)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 11:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    Prepare the 2.5.1 release
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
        Created At 2023-01-11 11:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    Fix the chaincode builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses a regression introduced in grpc-js:1.8.2, pinning the dependency to 1.8.1.

Previously the fabric-shim had a loose dependency on `^1.4.1`, which caused errors when the grpc-js runtime was updated with [this PR](https://github.com/grpc/grpc-node/pull/2316) 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 15:19:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Publish multi-arch, arm64 docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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

