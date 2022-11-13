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
                PR <a href="https://github.com/hyperledger/besu/pull/4667" class=".btn">#4667</a>
            </td>
            <td>
                <b>
                    Release 22.10.1 alpha, bonsai snapshot fix
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
squash commit of #4666  for 22.10.1-alpha

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-13 08:17:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4666" class=".btn">#4666</a>
            </td>
            <td>
                <b>
                    Fix for block unavailability during SnapshotTrieLog  caching
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
When blocks execute and their worldstates are appended as trie logs, the blocks are not yet available in blockchain storage.  Blockheaders are required to create/roll a snapshot trie log to a particular state. This PR changes the SnapshotTrieLogManager to create mutable snapshots once  blocks are appended to the chain.

This fix:
* directly addresses a snapshot transaction memory leak, rather than relying on finalize() methods in #4645 
* should be more performant since mutable copies are correctly cached rather than created
* decreases GC pressure since snapshots are closed correctly ahead of GC

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #4637 
fixes #4643 


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-13 08:03:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4665" class=".btn">#4665</a>
            </td>
            <td>
                <b>
                    Release 22.10.1 alpha
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
build for 22.10.1-alpha

merges `main`
also speculatively merges (in commit order):
 * #4644 
 * #4655 
 * #4656 
 * #4600
 * #4648



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-12 20:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4664" class=".btn">#4664</a>
            </td>
            <td>
                <b>
                    make snapshots the default for bonsai
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
inverts the default value for `--Xbonsai-use-snapshots` to true.  
adjusts some worldstate archive tests

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-12 20:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4662" class=".btn">#4662</a>
            </td>
            <td>
                <b>
                    squash commit of push0, small EOF
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

squash commit of 4460 and 4644
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-12 03:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4661" class=".btn">#4661</a>
            </td>
            <td>
                <b>
                    22.10.1 alpha
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

alpha build for burn in ahead of 22.10.1 release.  

This PR:
* merges main from e7074c0ecb582b50055c1928da85a2e79e9f97ba into release-22.10.x 
* sets gradle.properties version to 22.10.1-alpha

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 23:41:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4660" class=".btn">#4660</a>
            </td>
            <td>
                <b>
                    Implementation of  PUSH0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: lukelee-sl <luke.lee@swirldslabs.com>


## PR description
Implement PUSH0 operation as described in https://eips.ethereum.org/EIPS/eip-3855

## Fixed Issue(s)
#4658 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 22:26:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4659" class=".btn">#4659</a>
            </td>
            <td>
                <b>
                    Fix circleCI snapshot segfaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                explicitly close snapshot worldstates and their copies to avoid a segfault on circle-ci when running BonsaiSnapshotIsolationTest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 21:54:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4657" class=".btn">#4657</a>
            </td>
            <td>
                <b>
                    Ignore .idea directory in spotless checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

InteliJ allows to define templates for different files like Java classes, interfaces,... If those templates are saved in the project they are saved as `.java` files in a subdirectory of `.idea`.

Such a template looks for example like this:
```
#parse("Copyright Besu.java")
#if (${PACKAGE_NAME} && ${PACKAGE_NAME} != "")package ${PACKAGE_NAME};#end
public class ${NAME} {
}
```
Spotless currently tries to check this templates, because it is configured to analyze all Java files. This check will fail, because the templates are not valid Java code.

This PR excludes all the files in the `.idea` directory from the spotless check to avoid those false positives.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 15:41:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4656" class=".btn">#4656</a>
            </td>
            <td>
                <b>
                    Backward sync: use retry switching peer when fetching data from peers 
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

This PR is built on top of #4655, so please che it first.

Wait for at least one connected peer before starting the backwward sync, and use the retry mechanism that switches peer everytime it needs to retry to get data from peers, this helps reducing errors like the following ones, and makes the sync faster

```
Backward sync failed (org.hyperledger.besu.ethereum.eth.manager.exceptions.NoAvailablePeersException: Task failed: NO_AVAILABLE_PEERS). Current Peers: 1. Retrying in 5000 milliseconds...
```

```
Backward sync failed (org.hyperledger.besu.ethereum.eth.sync.backwardsync.BackwardSyncException: Did not receive a headers for hash 0xe4631c4449f24076d15c6ab3f663ac573ab4faa945aadbb85573848920e8ff80). Current Peers: 1. Retrying in 5000 milliseconds
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

relates to #4446 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 13:29:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4655" class=".btn">#4655</a>
            </td>
            <td>
                <b>
                    Backward sync log UX improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Improve the backward sync logging, showing only the progress and critical errors, and pushing transient errors to debug.
Progress logs are printed at least 10 sec apart, to avoid spamming the console

example of the new progress log

```
{"@timestamp":"2022-11-11T11:54:59,077","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"BackwardsSyncAlgorithm","message":"Backward sync target block is 2267767 (0x3e6762c92c604cf19e6ba6377a15a8266afdb6bca81b57b1c8d49b7bcc03571c)","throwable":""}                                                                                                                                                                                                                   {"@timestamp":"2022-11-11T11:55:51,964","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2, 1.56% completed, downloaded 200 headers of at least 12842. Peers: 1","throwable":""}                                                                                                                                                                                                                                    {"@timestamp":"2022-11-11T11:55:59,834","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2 completed, downloaded a total of 13000 headers. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:56:01,771","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 1.56% completed, imported 200 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:56:12,925","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 12.46% completed, imported 1600 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:56:22,934","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 21.80% completed, imported 2800 blocks of at least 12842. Peers: 3","throwable":""}
{"@timestamp":"2022-11-11T11:56:34,671","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 38.93% completed, imported 5000 blocks of at least 12842. Peers: 1","throwable":""}                                                                                                                                                                                                                                      {"@timestamp":"2022-11-11T11:56:45,305","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 52.95% completed, imported 6800 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:56:56,366","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 62.30% completed, imported 8000 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:57:06,473","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 71.64% completed, imported 9200 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:57:16,819","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 79.43% completed, imported 10200 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:57:28,240","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2, 91.89% completed, imported 11800 blocks of at least 12842. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:57:34,237","level":"INFO","thread":"nioEventLoopGroup-3-2","class":"ForwardSyncStep","message":"Backward sync phase 2 of 2 completed, imported a total of 12857 blocks. Peers: 1","throwable":""}
{"@timestamp":"2022-11-11T11:57:34,242","level":"INFO","thread":"ForkJoinPool.commonPool-worker-7","class":"BackwardsSyncAlgorithm","message":"The Backward sync is done","throwable":""}
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

relates to #4446

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 11:58:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4654" class=".btn">#4654</a>
            </td>
            <td>
                <b>
                    Adding option to debug the potential problems with closing Transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If we are adding finalize, at least add some way to investigate a potential not closed object. 

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 10:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4651" class=".btn">#4651</a>
            </td>
            <td>
                <b>
                    fix best peer mechanism during sync
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 16:24:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4650" class=".btn">#4650</a>
            </td>
            <td>
                <b>
                    Added 'result' field to eth_sendRawTransaction invalid transaction response.
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
Adds a `result` field (containing the transaction hash) to the response from `eth_sendRawTransaction` when the transaction is invalid. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 12:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4649" class=".btn">#4649</a>
            </td>
            <td>
                <b>
                    Upgrade RocksDB from version 7.6.0 to 7.7.3
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
The new version of RocksDB JNI library was published in maven on Oct 25, 2022, this PR will upgrade rocksdb JNI library from 7.6.0 to 7.7.3.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 09:45:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4648" class=".btn">#4648</a>
            </td>
            <td>
                <b>
                    Bonsai Fix for MainnetBlockValidator
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
Fix for MainnetBlockValidator mutating the bonsai persisted worldstate on validation.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 09:06:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4647" class=".btn">#4647</a>
            </td>
            <td>
                <b>
                    add bandersnatch point
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This adds just enough code to deal with the math required to create verkle proofs.


## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 07:43:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4646" class=".btn">#4646</a>
            </td>
            <td>
                <b>
                    WIP: Implement eth/67 sub protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 03:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4645" class=".btn">#4645</a>
            </td>
            <td>
                <b>
                    Ensure snapshots released before gc
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
Short term fix to ensure snapshot transactions are closed and snapshots released before their respective objects are GC'd.

This is a stop-gap measure until a subsequent PR addresses #4641 and can use static analysis to ensure all worldstates are closed at the end of their lifecycle.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes  #4643 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 03:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4644" class=".btn">#4644</a>
            </td>
            <td>
                <b>
                    "Small" Ethereum Object Format (EIP-3540 + EIP-3670)
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
Implement "Small" EOF - EIP-3540 (container) and EIP-3670 (validation).

Make code an interface so EOF specific features are compartmentalized,
including an 'invalid' code type representing a code block that didn't
pass validation, CodeV1 for EOF1, and CodeV0 which represents pre-EOF
code. EVMs track a maximum supported EOF version (where 0 is pre-eof)and
code is generated from a CodeFactory taking in context (is it a CREATE
operation and max code size) for the validation.

Includes spec versions for "Shanghai" and transient testnet "Shandong".

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 00:59:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4642" class=".btn">#4642</a>
            </td>
            <td>
                <b>
                    Replace quadruplicated anonymous  implementation of SubProtocol with MockSubProtocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
Refactoring: Replace quadruplicated anonymous  implementation of SubProtocol with MockSubProtocol

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 00:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4640" class=".btn">#4640</a>
            </td>
            <td>
                <b>
                    ♻️ Refactor EthProtocol to externalise EthVersion into its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor EthProtocol to externalise EthVersion into its own class to improve readability

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 22:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4635" class=".btn">#4635</a>
            </td>
            <td>
                <b>
                    Optimize performance of WorldStateUpdater commit method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
Co-authored-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
WorldStateUpdater commit method is one of the most consuming methods during block processing (engine_newPayloadV1 call). This PR will focus on parallelizing some parts of this method to make it faster.

<img width="1714" alt="image" src="https://user-images.githubusercontent.com/5099602/200810024-878e01e0-3f54-4911-9157-0bd73be1cb3f.png">

The first results after 2 hours of execution

<img width="1332" alt="image" src="https://user-images.githubusercontent.com/5099602/200866595-4057e7be-3cf1-4153-a9e0-59b33c861d6f.png">

The results after 12 hours
<img width="1621" alt="image" src="https://user-images.githubusercontent.com/5099602/201040164-b39ac12d-734d-45e8-a718-295edd94b886.png">

We can see with CPU profiling that the commit methods takes less time and most of the execution is done in parallel in ForkjoinPool.commonPool().

<img width="1707" alt="image" src="https://user-images.githubusercontent.com/5099602/201041208-aa00707e-7b20-4444-9ff6-2ef68fe5d6ed.png">

<img width="1712" alt="image" src="https://user-images.githubusercontent.com/5099602/201042608-296742ab-15c6-4aad-8904-55db8ae68a20.png">


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Mitigate #4549

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 10:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    WIP QBFT Empty Block Period
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
#3810 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 04:36:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4633" class=".btn">#4633</a>
            </td>
            <td>
                <b>
                    Remove SHL, SHR and SAR from default EVM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
This PR removes the opcodes `SHL`, `SHR` and `SAR` from the base EVM b/c those were added in [EIP-145](https://eips.ethereum.org/EIPS/eip-145) and shouldn't be available since Genesis.

## Fixed Issue(s)
Spotted by @winsvega during the execution of LegacyTests. E.g.
```shell
$ ./retesteth -t LegacyTests/Constantinople/BCGeneralStateTests/stShift -- --singletest shr11_d0g0v0 --clients besu --singlenet Byzantium --nodes 127.0.0.1:8545
```

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Diego López León <dieguitoll@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 17:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    Refactor transaction pool tests
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

Refactor and improve transaction pool unit tests.

- removed code duplication
- created an abstract class and 2 concrete impementations one for the legacy fee market, and the other one for the London fee market, so it is easier to reason about tests that common and specific tests

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 10:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4627" class=".btn">#4627</a>
            </td>
            <td>
                <b>
                    Bonsai commit updater optimization investigation
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 17:34:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4622" class=".btn">#4622</a>
            </td>
            <td>
                <b>
                    Make Json RPC TLS Test Java 17 friendly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

There was a change in error codes in Java DER decoding between Java 17 and Java 11.  Tests depend on Java 11 error.  Use JUnit5 facilities to ensure the test works proeprly on both with the same codebase.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 16:27:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4620" class=".btn">#4620</a>
            </td>
            <td>
                <b>
                    Warm Coinbase (EIP-3651)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add a flag to MainnetTransactionProcessor to add the miningBeneficiary to the list of pre-warmed addresses.
Have shandong fork set this flag to true by default.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 16:19:19 +0000 UTC
    </div>
</div>

