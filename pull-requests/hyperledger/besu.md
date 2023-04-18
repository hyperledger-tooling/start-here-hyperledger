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
                PR <a href="https://github.com/hyperledger/besu/pull/5352" class=".btn">#5352</a>
            </td>
            <td>
                <b>
                    Add new sepolia bootnodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Same as #5347 just with DCO and other unit test fixed. Happy to add @paritosh as co-author.



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
From #5347 
> Sepolia has had some peering troubles in the past, It seems like the old EF bootnodes weren't created properly or not added to the IaC stack we usually have our configs in, so I went ahead and setup new bootnodes on DigitalOcean. These have more liberal bandwidth limits and cost far lesser to run, they should be able to help with peering and sync performance on Sepolia.
The bootnode configs have been commited to the private devops repo along with a reserved IP and the nodekey has been backed up. The bootnode has additionally been added to the DevOps monitoring and updating stack. We should be able to maintain these bootnodes far better in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 06:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5350" class=".btn">#5350</a>
            </td>
            <td>
                <b>
                    uncomment columns related to GoQuorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses database backwards compatibility broken by https://github.com/hyperledger/besu/commit/067a26337411833ad92d649f208255b1a7954268

Fixes `org.rocksdb.RocksDBException: Column families not opened:` error

See #5303
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-16 22:20:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5349" class=".btn">#5349</a>
            </td>
            <td>
                <b>
                    [MINOR] Add database compatibility to the PR checklist
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
        Created At 2023-04-16 21:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5346" class=".btn">#5346</a>
            </td>
            <td>
                <b>
                    Improved error message when verifying enode syntax with xdns-enabled
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
Improved error message when verifying enode syntax with xdns-enabled

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/2569
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 06:41:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5344" class=".btn">#5344</a>
            </td>
            <td>
                <b>
                    [MINOR] fix Javadoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add missing javadoc 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 01:18:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5343" class=".btn">#5343</a>
            </td>
            <td>
                <b>
                    Upgrade Reference Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade reference tests to v12.1

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
        Created At 2023-04-13 22:16:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5342" class=".btn">#5342</a>
            </td>
            <td>
                <b>
                    updating issue template requesting logs
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
Update to request logs in the issue template 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 20:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5340" class=".btn">#5340</a>
            </td>
            <td>
                <b>
                    [MINOR] Remove ENGINE_EXECUTE_PAYLOAD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                Think this was renamed to engine_newPayloadV1 so not actually used by anything currently

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes https://github.com/hyperledger/besu/issues/5336
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 06:44:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5339" class=".btn">#5339</a>
            </td>
            <td>
                <b>
                    Remove RocksDb deprecated option maxBackgroundCompactions 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR cleans up the besu rocksDB plugin removing all the `maxBackgroundCompactions` usage. Might be useful to get a following PR to introduce `maxBackgroundJobs` if we still want to support this type of customisation in the plugin


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 04:33:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5338" class=".btn">#5338</a>
            </td>
            <td>
                <b>
                    Set version as 23.1.3 and minor changelog update
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
        Created At 2023-04-13 02:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5337" class=".btn">#5337</a>
            </td>
            <td>
                <b>
                    Updating confusing --bonsai-maximum-back-layers-to-load option to --bonsai-historical-block-limit + remove deprecated snapshots config 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Changed the mentioned flags. Alias used to keep backwards compatibility. Also removed now deprecated snapshots option. 

## Fixed Issue(s)
Ambiguity 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 20:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5335" class=".btn">#5335</a>
            </td>
            <td>
                <b>
                    Update OpenJ9 Docker image
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
Update OpenJ9 docker image to Ubuntu 22.04 as a base image.
I have different performance results depending on the OS. OpenJ9 x86_64 docker image has better block processing time that running natively Besu with a Hotspot JVM. The screenshots below are from AWS instances m6a.2xlarge

![image](https://user-images.githubusercontent.com/5099602/232448468-d673a01d-8a78-4525-b5a7-e7ddabc445e9.png)

OpenJ9 JVM demonstrates significantly lower memory usage compared to HotSpot JVM, resulting in a reduction of 6 GiB in this particular scenario.

![image](https://user-images.githubusercontent.com/5099602/232454738-4c6b4c02-abfe-4c69-96d5-8a50b7cf3c29.png)


OpenJ9 aarch64 docker image block processing is 6% slower than a hotspot docker image (on aarch64). 

![image](https://user-images.githubusercontent.com/5099602/232451707-a5d30b2b-1983-47de-9a0a-5ab0bfca2928.png)

Despite the HotSpot JVM's ability to free up memory, OpenJ9 still showcases very low memory usage on aarch64 architecture. Although HotSpot has caught up with OpenJ9 and now consumes a similar amount of memory, OpenJ9 remains a solid choice for those looking to minimize their memory footprint.

![image](https://user-images.githubusercontent.com/5099602/232455019-8c88fe6f-c1ed-4805-bd8c-9834ede234b0.png)

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5327

<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 10:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5334" class=".btn">#5334</a>
            </td>
            <td>
                <b>
                    Update version to 23.4.0-SNAPSHOT
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
Update main version to 23.4.0-SNAPSHOT ready for the next release so we can use 23.1.3-SNAPSHOT on the [release-23.1.x](https://github.com/hyperledger/besu/tree/release-23.1.x) branch

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 08:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5331" class=".btn">#5331</a>
            </td>
            <td>
                <b>
                    Reduce UInt256 in EVMOperations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Improve the performance of the EVM by reducing the usage of UInt256 in almost all operations and moving the main switch to a Java 17 expression switch

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 16:21:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5330" class=".btn">#5330</a>
            </td>
            <td>
                <b>
                    Update get account method in the accumulator
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

Update get account method in the accumulator in order to not use the cache in this case


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 15:51:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5329" class=".btn">#5329</a>
            </td>
            <td>
                <b>
                    Add javadoc
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
        Created At 2023-04-11 14:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5328" class=".btn">#5328</a>
            </td>
            <td>
                <b>
                    Rocksdb plugin to support OptimisticTransactionDb and TransactionDb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Tis PR introduces some changes to the RocksDB plugin to allow using the DB in either pessimistic or optimistic transaction mode.
Currently pessimistic is tied to the usage of Forest data format.

The refactor was done with the intent to keep bonsai as it is currently with usage of the optimistic transaction db.

This is just a initial draft not ready for review yet. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Partially fixes #5300 

Scenarios tested:

**Sepolia**
- [x] Fast-sync Forest (uses Pessimistic mode)
- [x] Snap-sync Bonsai (uses Optimistic mode)   

**Goerli**
- [x] Fast-sync Forest (uses Pessimistic mode)
- [x] Snap-sync Bonsai (uses Optimistic mode)

**Mainnet**
- [ ] Snap-sync Forest (uses Pessimistic mode) not finished yet
- [x] Snap-sync Bonsai (uses Optimistic mode)
- [ ] Checkpoint-sync Forest (uses Pessimistic mode) not finished yet 
- [x] Checkpoint-sync Bonsai (uses Optimistic mode)

**Backwards compatibility**
- [x] Roll back a Forest synced node to 23.1.2 forcing it to use Optimistic 
- [ ] Update a current synced Forest node that is using Optimistic to use the new version with pessimistic to ensure this won't require resyncs. (not done yet) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 11:45:32 +0000 UTC
    </div>
</div>

