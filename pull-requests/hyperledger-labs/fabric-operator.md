---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Launch the sample network on Apple Silicon;  Pin k8s to 1.24
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows the sample network to run correctly (albeit, slowly) on the new Mac Silicon / arm64 chipset.

The docker images run as `linux/amd64` under QEMU, so performance is very slow.  We should improve the build pipeline to support the `buildx` builder and generate multi-arch containers. 

This PR addresses Issue #63 by pinning the KIND target revision to 1.24.4 (`KIND_CLUSTER_IMAGE`). 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 11:31:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    cleanup: remove BoolTrue and BoolFalse variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 08:04:00 +0000 UTC
    </div>
</div>

