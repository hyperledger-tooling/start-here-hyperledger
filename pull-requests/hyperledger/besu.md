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
                PR <a href="https://github.com/hyperledger/besu/pull/4433" class=".btn">#4433</a>
            </td>
            <td>
                <b>
                    post-22.7.3 changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

post-release changelog update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 17:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4432" class=".btn">#4432</a>
            </td>
            <td>
                <b>
                    these don't need to be at info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 17:30:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4431" class=".btn">#4431</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.7.4-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.7.4-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 16:57:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4430" class=".btn">#4430</a>
            </td>
            <td>
                <b>
                    Release 22.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.7.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 16:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4427" class=".btn">#4427</a>
            </td>
            <td>
                <b>
                    add engine_preparePayload_debug endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Draft PR to enable debugging block proposals by re-adding an updated version of the deprecated 
`engine_preparePayload` endpoint

*be sure to use the current or a recent parent blockhash or you will DoS bonsai db*
example usage:
```
curl --location --request POST 'http://localhost:8551' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2NTkwNDEzMzZ9.4PDdSaG9hFOFR4Th7rEgaKKECsXfz6IPckFRcfSP13o' \
--data-raw '{
    "jsonrpc":"2.0",
    "method":"engine_preparePayload_debug",
    "params":
    [
        {
            "parentHash": "0xd4e56740f876aef8c010b86a40d5f56745a118d0906a34e69aec8c0db1cb8fa3",
            "feeRecipient": "0x0000000000000000000000000000000000000000",
            "timestamp": "0x0",
            "prevRandao": "0x0"
        }
    ],
    "id":1
}'
```



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
        Created At 2022-09-22 21:34:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4426" class=".btn">#4426</a>
            </td>
            <td>
                <b>
                    update CHANGELOG for 4349
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 16:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4425" class=".btn">#4425</a>
            </td>
            <td>
                <b>
                    Transaction pool improvements to avoid filling the pool with not executable transactions
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

This PR is built on top of #4413 which was used to investigate the transaction pool, with the result that currently we keep many transactions that are not possible to include in a block, because a transaction with a lower nonce is missing or invalid.
To avoid that issues first we now remember (in a cache) that that sender has an invalid transaction, and we do not accept transactions with higher nonce from that sender, of course if a replacement for the invalid transaction is sent it is accepted.
The eviction when the pool is full has changed in order to pick the sender of the oldest transaction in the pool, and the evict the transaction with the higher nonce for that sender, so no gaps in the nonce list for that sender are created.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #4401 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 15:20:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4423" class=".btn">#4423</a>
            </td>
            <td>
                <b>
                    Create a new flag on RocksDB for high spec hardware to boost performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Create a new flag on RocksDB (_--Xplugin-rocksdb-high-spec-enabled_) for high spec hardware to boost performance. 
With this first version, the impact is on memory usage, as we're tuning RocksDB block cache and Memtables size. By high spec here, we mean a VM or machine with more than 16 GiB. Other modifications in future may include other resources' requirements but for now, the only requirement is on RAM.

The results are promising on a 32 GiB AWS VM, as this new flag reduces 95 percentile block processing time by 30%.
![image](https://user-images.githubusercontent.com/5099602/191719256-14a0b56d-9fa7-4164-aada-b472fcf8adf7.png)

Performance improvements may appear in a couple of hours because of cache warm up time, as we can notice with RocksDB block cache hit ratio and RocksDB get time :

![image](https://user-images.githubusercontent.com/5099602/191847101-1093cc5f-60e7-466f-b6de-7fed273c8a15.png)
![image](https://user-images.githubusercontent.com/5099602/191847138-0d4c95ac-122c-4c5c-b61c-ae71de3a5301.png)

 
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
        Created At 2022-09-22 10:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4420" class=".btn">#4420</a>
            </td>
            <td>
                <b>
                    Change min selection to an unsigned min
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Change the "minimum" gas in the TangerineWhistleGasCalculator to use an unsigned comparison, to ensure a larger signed value is not selected.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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
        Created At 2022-09-21 16:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4419" class=".btn">#4419</a>
            </td>
            <td>
                <b>
                    Upgrade snakeyaml to 1.32
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Upgrade org.yaml:snakeyaml to 1.32

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>


## Fixed Issue(s)

Fixes #4418 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 15:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4417" class=".btn">#4417</a>
            </td>
            <td>
                <b>
                    Make transaction pool limits for sender based on pool size
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
Limit the portion of the transaction pool that a single sender can occupy to a percentage
* defaults to 0.1%, or default of 5 per sender with default max txpool size
* moves this config out of BesuCommand and into TransactionPoolOptions

This PR will see the default txpool configuration restrict the number of transactions from a single sender in the pool from 64 to 5.  This should decrease the cost of transaction eviction during transaction processing, and yield a transaction pool with a greater percentage of executable transactions for building a block.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #4401 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 08:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4416" class=".btn">#4416</a>
            </td>
            <td>
                <b>
                    Bump besu-native to 0.6.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Bump besu-native to 0.6.1 in order to get bls12-381 lib for linux arm64

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
        Created At 2022-09-21 05:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4415" class=".btn">#4415</a>
            </td>
            <td>
                <b>
                    Remove sender from map when he has no more tracked transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

In the transaction pool a sender is tracked when he has transactions, but he is never removed from the internal tracking data structure when he has no more transactions in the pool, so once a sender is added he lives forever in the pool even if he has no transactions there.
This PR remove the sender from the internal map when his last transaction is removed.

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
        Created At 2022-09-20 17:52:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4412" class=".btn">#4412</a>
            </td>
            <td>
                <b>
                    WIP - Copying storage to flat database for one account
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
        Created At 2022-09-19 23:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4411" class=".btn">#4411</a>
            </td>
            <td>
                <b>
                    Less strict engine QoS timer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Resets engine QoS timer with every call to the engine API instead of only when `ExchangeTransitionConfiguration` is called. `ExchangeTransitionConfiguration` mismatch will only submit a debug log not a warning anymore.

## Fixed Issue(s)
fixes #4404

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 14:35:10 +0000 UTC
    </div>
</div>

