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
With this first version, the impact is on memory usage, as we're tuning RocksDB block cache and Memtables size.

The results are promising on a 32 GiB AWS VM, as this new flag reduces 95 percentile block processing time by 30%.
![image](https://user-images.githubusercontent.com/5099602/191719256-14a0b56d-9fa7-4164-aada-b472fcf8adf7.png)

Add more tests for 16 GiB VM ...

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
                    Remove sender from map when he has no more tracked transaction
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
                PR <a href="https://github.com/hyperledger/besu/pull/4413" class=".btn">#4413</a>
            </td>
            <td>
                <b>
                    Add more tracing logs to transaction pool
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

This PR only adds trace logs that are useful for debbuging the empty blocks issues, indeed using these new trace logs it was possible to improve the transaction pool in #4425 

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
        Created At 2022-09-20 10:59:25 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4410" class=".btn">#4410</a>
            </td>
            <td>
                <b>
                    Fix Besu StacklessClosedChannelException errors and resulted Timeout errors in CL clients
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
StacklessClosedChannelException are thrown when some Eth calls, like eth_syncing or eth_getBlockByHash have to wait for the engine_newPayloadV1 call to finish. As the latter takes sometimes more than 1 second to execute depending on the block size, transactions type and hardware setup, the CL closes the connection [(in the case of Lighthouse)](https://github.com/sigp/lighthouse/pull/3470) because the timeout is set to 1 second on these calls.

In the screenshot below, we can see that 1 eth_getBlockByHash call and 2 eth_syncing calls are waiting for engine_newPayloadV1 call to finish.

![image](https://user-images.githubusercontent.com/5099602/190864397-407e85f9-b801-4ebd-8d2d-1606628e9321.png)

The Eth calls should't execute sequentially with the other Engine API calls, this fix will make several requests to execute concurrently on port 8551. 
@garyschulte please confirm that the 'Engine" will still execute sequentially even with this new configuration.

You can find lighthouse logs [before](https://gist.github.com/ahamlat/8ccdaf24c6524d377fdfff973fa5307b) and [after](https://gist.github.com/ahamlat/aff44be042e57a72729ee693d446eabf) the fix.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4398 and #4400 
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-17 15:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4409" class=".btn">#4409</a>
            </td>
            <td>
                <b>
                    Bonsai snapshot worldstate 
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
This PR adds support for using rocksdb snapshot transactions as the basis for a bonsai worldstate.  This gives us the ability to have an isolated copy of the world state for concurrent operations like block production, block validation, transaction validation, historical state queries, etc.

The notion is to merge this capability into main, and start replacing the uses of BonsaiLayeredWorldState and direct uses of BonsaiInMemoryWorldState when we need isolated and/or concurrent operations on the worldstate.

This is a strictly additive PR and does not change existing implementations.  Uses of snapshot worldstates will be useful to resolve issues such as #4372 #4250 #4199 #4151 and other bonsai concurrency issues.

Changes in support of snapshot worldstate include:
* moving (back) to OptimisticTransactionDB, so we can mutate the snapshot transactions
* creating `BonsaiWorldStateKeyValueStorage.BonsaiUpdater` interface extending `WorldStateStorage.Updater`, so we can have a snapshot specific Updater implementation
* Addition of SnappableStorage, SnappedStorage to plugin-api in order to support/expose the snapshot behavior 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #4402 
relates to #4403 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 21:48:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4407" class=".btn">#4407</a>
            </td>
            <td>
                <b>
                    Retry mechanism for block creation
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

Retry block creation if there is a transient error and we still have time, to mitigate empty block issue, as describe here
https://github.com/hyperledger/besu/issues/4401#issuecomment-1249340589

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

mitigates #4401 when there is a `org.rocksdb.RocksDBException: TimedOut(LockTimeout)`

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 17:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4406" class=".btn">#4406</a>
            </td>
            <td>
                <b>
                    Add Rpc method name when logging IOException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add Rpc method name when logging IOException

## Fixed Issue(s)
fixes #4405 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 05:51:03 +0000 UTC
    </div>
</div>

