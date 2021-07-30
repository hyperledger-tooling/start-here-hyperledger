---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2799" class=".btn">#2799</a>
            </td>
            <td>
                <b>
                    Gateway enabled by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In readiness for the Beta release, set the ‘Enabled’ config option of the gateway to ‘true’.
All peers will now have the gateway server enabled unless it is explicitly disbaled.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 13:47:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2796" class=".btn">#2796</a>
            </td>
            <td>
                <b>
                    Update doc for default chaincode instantiation policy (release-1.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update doc to indicate that default chaincode instantiation policy
is any channel admin.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 20:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2793" class=".btn">#2793</a>
            </td>
            <td>
                <b>
                    [FAB-11334] Adds a viper Cmd to unjoin a peer from a channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a Viper cobra.Command to unjoin the peer from a specified channel.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

This PR introduces a `node unjoin` cobra.Cmd to the peer binary.  When enjoining a channel, the peer must be shut down, and the command will scrub all channel artifacts from the kvledger and transient storage.   If a crash occurs during the removal of the ledger, the residual artifacts will be scrubbed at the next launch of the peer. 

#### Additional details

PR #2769 
PR #2754 
PR #2732 

#### Related issues

[FAB-16035](https://jira.hyperledger.org/browse/FAB-16035)
[FAB-4481](https://jira.hyperledger.org/browse/FAB-4481)
[FAB-17787](https://jira.hyperledger.org/browse/FAB-17787)
[FAB-17801](https://jira.hyperledger.org/browse/FAB-17801)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 11:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    FAB-18067 Discovery support Implicit Collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Implemented the fix as suggested by Yacov in his Jira comment.

Verified the fix works against the asset-transfer-secured-agreement sample which uses implicit collections.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 12:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Update to latest major version of Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-24 23:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2780" class=".btn">#2780</a>
            </td>
            <td>
                <b>
                    FAB 18365 IT flake evictionsuspector failed to read eviction 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Description
In failing case, the OSN being removed has committed the config change but failed to receive apply_config msg to halt the chain. This state is defined to be handled as part of the eviction suspicion logic. But it failed when evictionsuspector failed to check from lastconfig block if chain is up-to-date. 

Fix: Updated the order of statements which looks at the latest config block and block height validation.

#### Type of change
- Bug fix

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 11:02:47 +0000 UTC
    </div>
</div>

