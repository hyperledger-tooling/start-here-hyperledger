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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    IOU deployment exercise
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 13:48:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    fabric-sdk: cleanup ordering connection on failure + retry #377
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-27 05:18:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    fabric-sdk: do not add resolvers for Fabric peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">cleanup</span>
            </td>
            <td>
                This PR updates NWO to remove from the resolvers references to Fabric peers.
The FPC integration was relaying in these resolvers. To fix this, the PR updates the FPC integration to leverage Fabric Discovery.

In addition, a flaky unit-test has been disabled.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    Remove need for GOPATH to be set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If GOPATH is set and fabric-smart-client is a subdir in that GOPATH then it must still follow the pattern
src/github.com/hyperledger-labs/fabric-smart-client

GOPATH can be set and not contain fabric-smart-client (means the go module cache can be stored elsewhere)

GOPATH not being set will default to $HOME/go and above rules apply

It still requires to be checked out as fabric-smart-client still though, see TODO

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 07:17:52 +0000 UTC
    </div>
</div>

