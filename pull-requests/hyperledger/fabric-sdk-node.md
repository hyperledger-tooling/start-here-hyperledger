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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    FABN-1715: Always check all files for license headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the list of files to check was obtained by diffing the last git commit, which produced an empty list in PR builds within Azure Pipelines and allowed PR builds to pass with missing license header.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 13:06:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    [FABN-1710] Fix HSM Persistence issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The original contributed PR #450 built on top of the current implementation to try to address this problem, however a fix applied by #392 actually incorrectly tried to persist the object handle into the wallet and this was changed to allow it to store the SKI and unfortunately the contributed PR built on top of this.

This PR removes a lot of what #392 did because the node-sdk HSM support is limited to a subset of HSMs currently where it's possible to identify an object handle by the Fabric SKI of the public key (ie so it's possible to set this after an object has been created in the HSM, which excludes AWS HSM for example). This doesn't need to be persisted into the wallet because it can easily be calculated from the persisted certificate.

This PR also addresses FABN-1713 because unnecessary code was introduced into the User implementation by #392 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 08:02:00 +0000 UTC
    </div>
</div>

