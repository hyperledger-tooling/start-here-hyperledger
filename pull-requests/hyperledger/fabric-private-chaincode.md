---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/642" class=".btn">#642</a>
            </td>
            <td>
                <b>
                    Upgrade parson
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                This PR upgrade our json implementation to the most recent version 1.2.1.

This updated version contains many security fixes and functional updates. In particular, parsing string values from json that contain multiple `\0` characters is now supported. This is pretty useful when dealing with standard Fabric composite keys.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 15:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Add stress test for many invocations and fix memory leak
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Test</span>
            </td>
            <td>
                Add another stress test to detect memory leaks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 17:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    Add del_state support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">comp/shim</span>
            </td>
            <td>
                This PR adds `del_state` to the FPC shim.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 17:10:40 +0000 UTC
    </div>
</div>

