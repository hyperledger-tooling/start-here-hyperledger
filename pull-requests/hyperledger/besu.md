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
                PR <a href="https://github.com/hyperledger/besu/pull/5428" class=".btn">#5428</a>
            </td>
            <td>
                <b>
                    Fix the number of RocksDB log files to 5 with 100 MB each
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix the number of RocksDB LOG files to 5 with 100 MB for each LOG file.
These logs are not to be confused with [number].log files which represent WAL files.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 10:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5426" class=".btn">#5426</a>
            </td>
            <td>
                <b>
                    Fix RocksDB missing metrics issue
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
I noticed that RocksDB metrics are no more exposed even when they are enabled.
This is a regression on main branch, this PR will fix this issue.

![image](https://user-images.githubusercontent.com/5099602/235882942-2f251d5d-8fd8-4cff-a51d-76e3d5665719.png)

## Fixed Issue(s)
#5427
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 09:37:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5425" class=".btn">#5425</a>
            </td>
            <td>
                <b>
                    Ban zero blob transactions
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

[An update to EIP-4844](https://github.com/ethereum/EIPs/pull/6863) made zero blob transactions invalid, so this PR adds the check to verify that at least one blob is specified, this check could be done statically when creating the transaction.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5401 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 09:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5424" class=".btn">#5424</a>
            </td>
            <td>
                <b>
                    Acceptance Test for Shanghai EVM changes (push0)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #5403

Splits Shanghai AT test cases out from paris.
Idea is to have an AT per "fork transition", i.e. ExecutionEngineShanghaiAcceptanceTest for paris -> shanghai
next one would be ExecutionEngineCancunAcceptanceTest for shanghai -> cancun

(Currently built on top of https://github.com/hyperledger/besu/pull/5423
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 08:45:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5423" class=".btn">#5423</a>
            </td>
            <td>
                <b>
                    Remove block creation task map entries when cancelling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Fixes potential memory leak - probably only significant for clients running lots of validators
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 07:12:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5422" class=".btn">#5422</a>
            </td>
            <td>
                <b>
                    Certificates - specify long expiry for intermediate certs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -validity 36500 needs to be specified for -gencert as well as -genkeypair

other changes to README are cosmetic

TODO - run through these commands to regenerate the certs used by the unit tests (suspect ATs may have the same problem - maybe we have not hit this issue there since they are running on nightly cadence)

see #5421 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 06:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5420" class=".btn">#5420</a>
            </td>
            <td>
                <b>
                    TEST 
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 02:28:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5419" class=".btn">#5419</a>
            </td>
            <td>
                <b>
                    Update sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update actions versions

Add workflow_dispatch


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 21:40:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5418" class=".btn">#5418</a>
            </td>
            <td>
                <b>
                    Transaction pool flag to disable specific behaviors for locally submitted transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Setting the option `tx-pool-disable-locals` transactions submitted via API `eth_sendrawtransaction` do not receive a special treatment and are validated like any remote transactions, and are not prioritized over remote transactions.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 19:45:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5410" class=".btn">#5410</a>
            </td>
            <td>
                <b>
                    Release 23.4.1-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

SNAPSHOT version, CHANGELOG updates, download links and artifact hashes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 17:54:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5409" class=".btn">#5409</a>
            </td>
            <td>
                <b>
                    uprevving to 23.4.0 for release
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
Building our 23.4.0 release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 17:01:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5408" class=".btn">#5408</a>
            </td>
            <td>
                <b>
                    allow custom module for json mapper
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

allow custom module for json mapper

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 14:55:45 +0000 UTC
    </div>
</div>

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
                <span class="chip">mainnet</span><span class="chip">RPC</span>
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
                <span class="chip">performance</span><span class="chip">mainnet</span><span class="chip">TeamChupa</span><span class="chip">forest</span><span class="chip">bonsai</span>
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

