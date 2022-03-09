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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Remove bash dependency from test network nano
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The scripts do not require bash so switch to sh and add shellcheck linting

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 12:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Java chaincode implementation  for ERC721 standard token.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Java HLF chaincode implementation of ERC721 is a standard. This standard is used for representing ownership of non-fungible tokens.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-06 04:53:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    Update test-network-k8s to use two digit version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instead of using the Fabric and Fabric CA three digit version (2.4.3),
utilize the two digit version (2.4).
Each time a Fabric/FabricCA release is pushed to dockerhub the two digit version tag is updated.
This approach simplifies maintenance so that scripts don't have to be updated for every
third digit release.

Apologies that the end of line character got updated in the IDE... the important change is in `test-network-k8s/network` file.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 22:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    fix addOrg3 for test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also added testing addOrg3 to build pipeline

closes #664 

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 16:02:00 +0000 UTC
    </div>
</div>

