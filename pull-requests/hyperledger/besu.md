---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5407" class=".btn">#5407</a>
            </td>
            <td>
                <b>
                    add proofs to blobs bundle 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add proofs to blobs bundle
Add blobBundle to GetPayloadV3
Todo: Possibly remove the EngineGetBlobsBundleV1 from the Engine API
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5398
Fixes #5399
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 07:55:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5406" class=".btn">#5406</a>
            </td>
            <td>
                <b>
                    Ensure parisSpecificModifications are unapplied for all subsequent forks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ...not just Shanghai

This is because you could have a genesis configured with e.g. cancunTime but leave shanghaiTime unconfigured.

Fixes #5404
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 05:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5405" class=".btn">#5405</a>
            </td>
            <td>
                <b>
                    Decompose putMilestone into putBlockNumberMilestone and putTimestampMilestone
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor refactor for readability and clarity.

Originally, I was trying to avoid timestamp or blockNumber details leaking outside of the ProtocolSchedule and its Builder.
I wanted to remove putMilestone from the public interface entirely, since for the mainnet use case, this detail can be kept inside the ProtocolScheduleBuilder. 
This would have meant building the milestones first and passing them into ProtocolSchedule's constructor, but this was not feasible given the way the ProtocolScheduleBuilder works, specifically the fact that ProtocolSpecBuilder relies on receiving a ProtocolSchedule which implies milestones must be added after the ProtocolSchedule itself has been constructed.

Since my original plan is not feasible, I think this is a better approach if we have to support a public put operation anyway.

Fixes #5354

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 04:10:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5397" class=".btn">#5397</a>
            </td>
            <td>
                <b>
                    Bug Fix eth_feeHistory - Issue-#4231 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix the eth_feeHistory response. Seems that more rewards, baseFeePerGas and gasUsedRatio are returned when highestBlock requested is lower than blockCount. This is due to the fact that for this case the range wasn't calculated properly and exceeded `resolvedHighestBlockNumber` with more than +1.
## Fixed Issue(s)
#4231 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 12:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5396" class=".btn">#5396</a>
            </td>
            <td>
                <b>
                    Add plugin API to select Transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
This PR adds an API that can be used to select Transactions while they are added to a block

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 06:10:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5392" class=".btn">#5392</a>
            </td>
            <td>
                <b>
                    remove zero lead bytes of log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span><span class="chip">mainnet</span><span class="chip">TeamChupa</span><span class="chip">bonsai</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 13:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5385" class=".btn">#5385</a>
            </td>
            <td>
                <b>
                    Permissioning - A better solution to fix NullPointerException on createPayload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is a more elegant solution then PR 5374 for issue 5370. When running on docker, URI returns null on getHost() method but returns the correct hostname on toString() method, owning to the 'underline character' on hostname in docker-compose services.

## Fixed Issue(s)
#5370 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 21:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5380" class=".btn">#5380</a>
            </td>
            <td>
                <b>
                    prepare main for next point release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
update changelog
prep for next point release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 20:25:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5379" class=".btn">#5379</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.0-RC2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.4.0-RC2-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 20:02:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5378" class=".btn">#5378</a>
            </td>
            <td>
                <b>
                    Burn-in release 23.4.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.0-RC1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 19:10:33 +0000 UTC
    </div>
</div>

