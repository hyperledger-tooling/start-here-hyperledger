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
                
            </td>
            <td>
                ## PR description
This PR aims to prevent accidental downgrade of Besu, which can potentially cause the DB to be irrevocably corrupted.

The approach I've used is as follows:

- Add a new `default` function `getBesuVersion()` to the `BesuService` interface that returns the class package implementation version of the `BesuService` class
  - This makes the Besu version string available to any plugin.
- Update `DatabaseMetadata` to have an optional `besuVersion` JSON property
  - This optionally adds `besuVersion` to the `DATABASE_METADATA.json` file written by the Rocks DB storage plugin
  - Also update the gradle prereqs to pull in `com.fasterxml.jackson.datatype:jackson-datatype-jdk8` to handle Java8 optional properties
- Update the Rocks DB `readDatabaseVersion()` function to check if the installed/runtime version is lower than the version recorded in `DATABASE_METADATA.json`, and throw a `StorageException` if it is
  - Update the gradle prereqs to pull in `org.apache.maven:maven-artifact` to provide access to the maven `ComparableVersion` class

Example `DATABASE_METADATA.json`:

```
{
  "version":1,
  "besuVersion":"23.10.4-dev-c9338660"
}
```

Any value after the first `-` character in the version number is ignored. This limits version comparison to the 3 calver digits, which I think is sufficient for DB protection checks. Any value after `-` isn't guaranteed to have a logical `compareTo` result, especially for `dev` or a commit hash.

The logic is as follows:
- If `besuVersion` isn't present then no check is made and startup proceeds. This ensures there are no issues when upgrading from a version that didn't record a `besuVersion`
- If `besuVersion` is present and is lower than the installed/runtime version, Besu updates it to have the latest version in it
- If `besuVersion` is present and is greater than the installed/runtime version, Besu fails to start because a lower version of Besu is being started than the version that most recently updated the file

## Remaining TODOs

- [ ] Update/add tests
- [ ] Add CLI arg such as `--allow-downgrade` to allow a downgrade if specified

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6303" class=".btn">#6303</a>
            </td>
            <td>
                <b>
                    Add --X-trie-log subcommand
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
This is a more direct approach to the previous attempt in #6188.
Tests showed that the previous attempt was taking too long (3 hours) to prune a 3.5 months old.

In this PR we "reset" the cf and load only the trielogs that we want to retain in the DB.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5390 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 04:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6302" class=".btn">#6302</a>
            </td>
            <td>
                <b>
                    Disable txpool during fullsync
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
        Created At 2023-12-14 15:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6300" class=".btn">#6300</a>
            </td>
            <td>
                <b>
                    create trie package for bonsai and forest
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

A PR to place Bonsai and Forest in the same trie package. This PR is a preparation for the introduction of Verkle. This trie package will have Verkle in a next PR and we will add a common package so that the different trie substructures can share classes if needed. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 10:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6299" class=".btn">#6299</a>
            </td>
            <td>
                <b>
                    [MINOR] Trailing peer limit log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">logging</span>
            </td>
            <td>
                fixes #6269 

```
sallymacfarlane@dev-elc-besu-teku-mainnet-dev-sally-trailing-peer-log-3:/var/log/besu$ grep Trailing besu.log
{"@timestamp":"2023-12-14T12:50:11,138","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xadb935a416b0c19aaf... with height 18783177","throwable":""}
{"@timestamp":"2023-12-14T12:51:47,696","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xc8a80e895f6b85f8ff... with height 18299999","throwable":""}
{"@timestamp":"2023-12-14T12:51:49,471","level":"DEBUG","thread":"nioEventLoopGroup-3-1","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0x48f462dab313723e05... with height 18001000","throwable":""}
{"@timestamp":"2023-12-14T12:52:19,523","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13883323","throwable":""}
{"@timestamp":"2023-12-14T12:52:40,702","level":"DEBUG","thread":"nioEventLoopGroup-3-4","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13885662","throwable":""}
{"@timestamp":"2023-12-14T12:52:49,897","level":"DEBUG","thread":"nioEventLoopGroup-3-2","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13886842","throwable":""}
{"@timestamp":"2023-12-14T12:53:19,501","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13889692","throwable":""}
{"@timestamp":"2023-12-14T12:53:49,340","level":"DEBUG","thread":"nioEventLoopGroup-3-3","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13891310","throwable":""}
{"@timestamp":"2023-12-14T12:54:19,841","level":"DEBUG","thread":"nioEventLoopGroup-3-10","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13893155","throwable":""}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 09:20:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6297" class=".btn">#6297</a>
            </td>
            <td>
                <b>
                    [MINOR] add genesis file name to config overview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">ux</span><span class="chip">non mainnet (private networks)</span>
            </td>
            <td>
                ```
# Configuration:                                                                                   #
# Network: Custom genesis file                                                                     #
# /Users/sm/workspace/besu/config/besu/genesis-linea.json                                          #
# Network Id: 59140                                                                                #
# Data storage: Forest                                                                             #
# Sync mode: Snap                                                                                  #
# RPC HTTP APIs: ADMIN,ETH,NET,WEB3,PERM,DEBUG,MINER,EEA,PRIV,TXPOOL                               #
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 06:32:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6296" class=".btn">#6296</a>
            </td>
            <td>
                <b>
                    [MINOR] Remove vintage engine dependencies where unused
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Remove the junit-vintage-engine dependency from several modules where it's not used
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 05:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6295" class=".btn">#6295</a>
            </td>
            <td>
                <b>
                    Snap sync client handle empty final account storage ranges
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

Bugfix snap sync edge case.  When snap syncing large contract storage, if the final requested range is empty, but there is an accompanying proof of exclusion, besu will not mark the request complete and will endlessly retry.

This PR handles this case by marking the request complete as long as there is an accompanying proof

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 22:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6293" class=".btn">#6293</a>
            </td>
            <td>
                <b>
                    move forest class to a specific package
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

This PR prepares for the introduction of the Verkle trie code. I start by cleaning up the worldstate section, moving and renaming everything that is forest into a specific package in order to clarify the difference between Bonsai and Forest in the code.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 14:55:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6289" class=".btn">#6289</a>
            </td>
            <td>
                <b>
                    Store trielog as blobdb
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
Store trielog as blobdb to improve performance.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See https://github.com/hyperledger/besu/issues/5866
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 07:49:21 +0000 UTC
    </div>
</div>

