---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    [helm] Adding Storage for DX Blobs and PVC Templating Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We aren't ensuring there's some sort of writeable filesystem to the DX pods for blob storage, might as well offer the ability to persist it too. This refactors how we template the DX PVCs to other more customization (size, storage class, etc.) for future users, as well as offers the ability to disable the PVCs and use `emptyDir` instead.

> **NOTE**: This does include a breaking change in the chart for how DX data is handled: `/data/peers` and `/data/peer-certs` are now apart of the same PVC but given subdirs within the volume. However, we have not made an official release of the chart yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 00:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/353" class=".btn">#353</a>
            </td>
            <td>
                <b>
                    Remove unique index on token URIs
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
        Created At 2021-12-08 22:10:14 +0000 UTC
    </div>
</div>

