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
                A change in v1.2.x and later versions of @grpc/grpc-js seems to be preventing client applications from exiting due to interval timers on the event queue created by @grpc/grpc-js/src/subchannel.ts. Reverting back to @grpc/grpc-js v1.1.8 seems to resolve the issue.

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    Release v2.2.7
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
        Created At 2021-06-17 14:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    FABN-1714: Fix JSDoc generation of Transaction class (release-2.2)
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
        Created At 2021-06-17 14:05:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    FABN-1714: Fix JSDoc generation of Transaction class
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
        Created At 2021-06-17 14:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    FABN-1714: Allow transactions to be serialized (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of change from main branch.

Transaction state can be serialized using Transaction.serialize(), and later reconstructed using Contract.deserializeTransaction(). This allows a transaction to be persisted and for the same transaction (including nonce and transaction ID) to be submitted again following a client application restart.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 11:06:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    FABN-1714: Exclude wallet files from license scan
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
        Created At 2021-06-17 09:38:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    FABN-1714: Allow transactions to be serialized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transaction state can be serialized using Transaction.serialize(), and later reconstructed using Contract.deserializeTransaction(). This allows a transaction to be persisted and for the same transaction (including nonce and transaction ID) to be submitted again following a client application restart.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 14:50:48 +0000 UTC
    </div>
</div>

