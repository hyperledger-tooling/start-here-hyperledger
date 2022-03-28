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
                PR <a href="https://github.com/hyperledger/besu/pull/3636" class=".btn">#3636</a>
            </td>
            <td>
                <b>
                    delete slice input data code
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
This code do not check whether the input value is not empty array. So, I changed this code as follows, I tried to connect the errors to EnclaveClientException.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3635

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 05:00:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3634" class=".btn">#3634</a>
            </td>
            <td>
                <b>
                    update rocksdbjni to v6.29.4 for compatibility with arm64 CPU architecture
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pedro Novais <jpvnovais@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Updates rocksdbjni dependency to v6.29.4 for compatibility with arm64 CPU architecture. 
It was tested on Apple M1 Pro 2021, OSx 12.3 

## Related Issue(s)
- #3540 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 23:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3633" class=".btn">#3633</a>
            </td>
            <td>
                <b>
                    Update reference tests to 0e8d25bb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## Fixed Issue(s)
fixes #3632 

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 22:37:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3631" class=".btn">#3631</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Performance test : bloom filter test
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
Performance test :
Enable RocksDB Bloom filter.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
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
        Created At 2022-03-25 13:24:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3629" class=".btn">#3629</a>
            </td>
            <td>
                <b>
                    Update the PR template to include a documentation checklist item.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: bgravenorst <byron.gravenorst@consensys.net>

## PR description
Updated the GitHub PR template to include a documentation checklist item.

## Fixed Issue(s)
Fixes #3628 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 01:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3626" class=".btn">#3626</a>
            </td>
            <td>
                <b>
                    Skip seen transactions
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

This is the last PR in the series to review and optimize transaction synchronization, and its goal is to avoid reprocessing transactions, that Besu have already seen recently.

The currently way Besu has to spot if a transaction has already been process, is to look if the transaction is present in the transaction pool, that by default is 4K, while the amount of pending transactions on the mainnet, is much more, the order of hundred of thousands, so basically even if a transaction has been already processed, the chances that it gets reprocessed is very high, with the result of doing a lot of useless work, that affects Besu performance.

A trivial solution could be to just raise the transaction pool size, but that is not always advisable, because it is critical for block production to keep it fast, and incresing its size could negatively affect the perfomance of the strategy choosen to select transactions to include in the block.

A better option, implemented in this PR, is to leverage data that we already have, and that keeps the history of the transactions exchanged with other peers. This data is just a collection of transaction hashes that we have received or seen, and in any case if a transaction is in that collection, it means that it has already been processed by Besu, so it is possible to directly skip it.

Tests show a reduced CPU usage:
![image](https://user-images.githubusercontent.com/91944855/159903502-35ad0aff-bfc8-4ab0-98c7-c0fdbc2503a5.png)
![image](https://user-images.githubusercontent.com/91944855/159903608-57ea1bdc-332f-42fc-aa35-7c3021e30d29.png)

due to the much less turnover in the transaction pool
![image](https://user-images.githubusercontent.com/91944855/159903959-c4bc1de1-ee3e-45ed-8f2f-6149a885a070.png)
![image](https://user-images.githubusercontent.com/91944855/159904240-adafdd71-4ad9-4f7b-8782-3770fb3f9479.png)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 17:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3625" class=".btn">#3625</a>
            </td>
            <td>
                <b>
                    init object for snapsync pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This is the first step initializing the snapsync pipeline. Setting up utility objects and request classes. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 15:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3623" class=".btn">#3623</a>
            </td>
            <td>
                <b>
                    adds validation that timestamp is after prior block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

## PR description
Adds check to make sure later blocks are after the last one.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3621 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 16:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3622" class=".btn">#3622</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Performance Test : Change RocksDB cache capacity from 8 MB to 64 MB.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performance Test :
Change RocksDB cache capacity from 8 MB to 64 MB.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
From CPU profiling metrics, we can notice that RocksDB.get consumes about 35% of CPU during fast sync.
As Block cache is where RocksDB caches data in memory for reads, we can increase this cache to reduce the complexity of reads.
This PR aims to test Besu Fast sync with RocksDB cache capacity of 64 MB (instead of the default value 8 MB).

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 16:04:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3620" class=".btn">#3620</a>
            </td>
            <td>
                <b>
                    Use JUnit 5 for unit test execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Change the unit test execution to use the Junit5 JUnitPlatform. This
allows for a mix of junit 4 and junit 5 tests and for a gradual
migration to junit 5 instead of a big bang. One class depended on
junit 4 exceptions and was updated.

Also, this facilitated a slight refactor of TLSContextFactoryTest so 
that when running on a mac (typical developer machine) errors stemming
from the nss3 library do not cause unit test failures, while still 
testing non-nss3 code paths. Tests will perform normally in integration.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 00:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3617" class=".btn">#3617</a>
            </td>
            <td>
                <b>
                    Return GOQUORUM_PRIVATE_STORAGE where it was
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should put back a missing GOQUORUM_PRIVATE_STORAGE enum that I accidentally removed.

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 14:51:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3616" class=".btn">#3616</a>
            </td>
            <td>
                <b>
                    Improve eth/66 support
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

Currently Besu has a limited support for sending NewPooledTransactionHashes messages, and other aspect related to reduce transactions synchronization traffic, described in the [Ethereum Wire Protocol](https://github.com/ethereum/devp2p/blob/master/caps/eth.md#ethereum-wire-protocol-eth) version 66.

Specifically:
1. Besu only uses NewPooledTransactionHashes for new local transactions, while it could be extended to any transaction added to the transaction pool
2. Besu does not limit the sending of the full transaction messages to a small fraction of the connected peers, and sends the new transaction hashes to all the remaining peers

This PR, extends eth/66 support and does some code refactoring, to remove some reduntant code and rename some classes to identify they are related to the NewPooledTransactionHashes message.

The main changes are:
1. Do not have a separate tracker for transaction hashes, since for them we can reuse PeerTransactionTracker, that tracks full transactions exchange history and sending queue with a peer. So PeerPendingTransactionTracker has been removed. `--tx-pool-hashes-max-size` is now deprecated and has no more effect and it will be removed in a future release.
2. When a new peer connects, if it support eth/6[56] then we send all the transaction hashes we have in the pool, otherwise we send the full transactions.
3. When new transactions are added to the pool, we send full transactions to peers without eth/6[56] support, or to a small fractions of all peers, and then we send only transaction hashes to the remaining peer that support eth/6[56]. Both transactions and transaction hashes are only sent if not already exchanged with that specific peer.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 13:44:21 +0000 UTC
    </div>
</div>

