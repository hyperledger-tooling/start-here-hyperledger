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
                PR <a href="https://github.com/hyperledger/besu/pull/6329" class=".btn">#6329</a>
            </td>
            <td>
                <b>
                    Copy also computed fields, when doing a Transaction detached copy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2023-12-22 15:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6328" class=".btn">#6328</a>
            </td>
            <td>
                <b>
                    Optimize RocksDB WAL file
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

Currently Besu uses the default RocksDB WAL options, with the result that usually the WAL files could occupy ~15GB of disk space, due to the fact that different column families are flushed at very different intervals, this has also the bad effect of slow restarts, when Besu has to parse an reapply all these WAL files.

Capping the WAL files total size to 1GB and reusing old files when possible, has the advantage of a faster restart, and a more linear disk usage, instead of the classic saw tooth shape that we see today.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 11:01:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6322" class=".btn">#6322</a>
            </td>
            <td>
                <b>
                    Cancun forkids for non-mainnets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add new forkids for testnets, update forkid test to Junit5, no longer need named network specific trusted setups


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 18:53:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6316" class=".btn">#6316</a>
            </td>
            <td>
                <b>
                    add missing check for static peers to allow them to exceed the connection limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In one place there was a check missing to allow static peers to exceed the connection limit.
Another improvement is that streamBestPeers() does only return fully validated peers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-20 02:13:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6315" class=".btn">#6315</a>
            </td>
            <td>
                <b>
                    Log/Address Trielog rolling failure
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
        Created At 2023-12-19 23:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6313" class=".btn">#6313</a>
            </td>
            <td>
                <b>
                    fix: call OperationTracer.traceEndTx for failing transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Call `OperationTracer.traceEndTx` even when a transaction failed.

## Fixed Issue(s)
fixes #6312 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 13:06:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6310" class=".btn">#6310</a>
            </td>
            <td>
                <b>
                    Release 23.10.3-RC4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RC3 failed on one specific canary; it ran into an edge case during a backwards sync on a single testing canary for lodestar on mainnet doing a checkpoint sync (see attached logfile, timestamp 2023-12-15T21:36:50,193 ). This did not happen for any other clients, including teku and sepolia variants.

There is a known issue in Besu where during a sync, a very tight loop will max out the CPU. We would like to add the fix for this issue to RC4.

[besu.log.zip](https://github.com/hyperledger/besu/files/13707409/besu.log.zip)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 19:19:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6309" class=".btn">#6309</a>
            </td>
            <td>
                <b>
                    Quick fix to avoid a tight loop when processing added blocks in txpool
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

When a node is full syncing or backward syncing, it is possible the processing of block added in the txpool, causes a tight loop, with the result of high cpu consumption, that causes the node to basically halt doing other tasks.
This is a quick workaround, while a proper solution, that also avoids to process added blocks during full sync is in progress, and will be ready.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 19:12:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6307" class=".btn">#6307</a>
            </td>
            <td>
                <b>
                    Restrict downgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
This PR aims to prevent accidental downgrade of Besu, which can potentially cause the DB to be irrevocably corrupted.

The approach I've used is as follows:

 - Add a new file `VERSION_METADATA.json` in the configured data path
   - Contains a single `besuVersion` field, e.g. `{"besuVersion":"23.10.3"}` 
 - Add a new `--allow-downgrade` configuration option
 - Update the gradle prereqs to pull in `org.apache.maven:maven-artifact` to provide access to the maven `ComparableVersion` class
 - Add a function `performDowngradeCheck()` to `VersionMetadata` as the first function to call after configuration options have been validated.
   - `performDowngradeCheck()` throws an exception if the version in `VERSION_METADATA.json` is higher (when compared using the maven `ComparableVersion` class) than the version as recorded in the `BesuCommand` class implementation version

Any value after the first `-` character in the version number is ignored. This limits version comparison to the 3 calver digits, which is all that can be logically compared as higher or lower. An example of a version number that has trailing characters is `23.10.4-dev-c9338660` where the latest commit has been appended to the version. The `-dev-c9338660` is ignored in the version comparison.

The validation logic is as follows:
- If the `VERSION_METADATA.json` file doesn't exist, no further checks are made and the node starts. The `VERSION_METADATA.json` file is written to allow version checks from this point onwards.
- If the file and `besuVersion` field are present and the version is lower than the installed/runtime version, Besu updates it to have the latest version in it and continues to start up
- If the file and `besuVersion` field are present and the version is greater than the installed/runtime version, Besu fails to start unless `--allow-downgrade` is set, because a lower version of Besu is being started than the version that most recently updated the file.

## Remaining TODOs

- [x] Update/add tests
- [x] Add CLI arg such as `--allow-downgrade` to allow a downgrade if specified

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6266
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 12:25:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6306" class=".btn">#6306</a>
            </td>
            <td>
                <b>
                    Generate genesis root hash with the used data storage format
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

Before, we always generated the root hash of the genesis with forest, even if we activated bonsai. I am modifying the logic to use the correct storage format that we activated. This will facilitate a potential removal of forest and also be able to generate the genesis root hash using verkle when it is integrate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 09:34:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6305" class=".btn">#6305</a>
            </td>
            <td>
                <b>
                    mark deleted slot during clear storage step
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
        Created At 2023-12-15 18:27:05 +0000 UTC
    </div>
</div>

