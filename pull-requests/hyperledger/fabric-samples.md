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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1040" class=".btn">#1040</a>
            </td>
            <td>
                <b>
                    Update FSAT to use Fabric 2.5 by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates full-stack-asset-transfer to Fabric 2.5 by default.

In particular, since k8s-builder-peer is set as the default value for peer image,
it needs to be updated to use 0.11.0, which is derived from Fabric v2.5 image, as the version default value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 08:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1039" class=".btn">#1039</a>
            </td>
            <td>
                <b>
                    Update test-network-k8s to Fabric v2.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates test-network-k8s to use Fabric v2.5.

This PR enhances the following PR.
https://github.com/hyperledger/fabric-samples/pull/1033

# Related Issues
- https://github.com/hyperledger-labs/fabric-builder-k8s/pull/92
- https://github.com/hyperledger/fabric-samples/issues/840
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 22:20:12 +0000 UTC
    </div>
</div>

