---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    Revert to snapshot publishing following release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 13:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Release v2.2.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 10:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/471" class=".btn">#471</a>
            </td>
            <td>
                <b>
                    FABN-1716: Fix hang on application exit (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of commit f59f91ce209f13b6bf03ad03135993728de7543f from main branch.

A change in v1.2.0 and later versions of @grpc/grpc-js is preventing client applications from exiting due to interval timers on the event queue created by @grpc/grpc-js/src/subchannel.ts. This appears to be linked to behaviour when the `grpc.keepalive_permit_without_calls` setting is enabled, which it is by default in the fabric-common configuration. This change disables that setting by default until a fix to @grpc/grpc-js is released.

Additionally, connection timeout Promises during sends to orderers in Committer.js were not being closed correctly. This did not cause a breakage since the promise they rejected was already resolved if the connection was successful, but could leave timers running unnecessarily in the event queue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 09:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    [FABN-1554] Add label support for HSM (#468)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the option to specify label instead of slot
If both are provided then slot will be ignored

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 07:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    FABN-1716: Fix hang on application exit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A change in v1.2.0 and later versions of @grpc/grpc-js is preventing client applications from exiting due to interval timers on the event queue created by @grpc/grpc-js/src/subchannel.ts. This appears to be linked to behaviour when the `grpc.keepalive_permit_without_calls` setting is enabled, which it is by default in the fabric-common configuration. This change disables that setting by default until a fix to @grpc/grpc-js is released.

Additionally, connection timeout Promises during sends to orderers in Committer.js were not being closed correctly. This did not cause a breakage since the promise they rejected was already resolved if the connection was successful, but could leave timers running unnecessarily in the event queue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 11:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    [FABN-1554] Add label support for HSM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the option to specify label instead of slot
If both are provided then slot will be ignored

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 11:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    Revert to snapshot publishing following v2.2.7 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 10:41:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    [FABN-1710] Fix HSM Persistence issues (#464)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Merged Pull request #450 into main
* Extend HSM tests

Signed-off-by: D <d_kelsey@uk.ibm.com>
Co-authored-by: Angel Kafazov <akafazov@cst-bg.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 14:22:27 +0000 UTC
    </div>
</div>

