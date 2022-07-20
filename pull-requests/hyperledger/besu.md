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
                PR <a href="https://github.com/hyperledger/besu/pull/4134" class=".btn">#4134</a>
            </td>
            <td>
                <b>
                    Add support for LevelDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fairly quick and dirty implementation of a LevelDB plugin for Besu. It does pass the `AbstractKeyValueStorageTest` tests but is pretty lacking in unit tests otherwise currently.  LevelDB doesn't support columns by default but this adds support via a key prefix - code for that is taken from Teku (and we could pull over the unit tests for it if this is worth pursuing).

It may be better to not simulate columns since I think besu always uses globally unique keys anyway (pruning needs the ability to iterate a single column but pruning isn't exactly useful anyway). That would likely simplify the implementation and may give different performance/space characteristics as well but I haven't tried it.

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 22:22:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4133" class=".btn">#4133</a>
            </td>
            <td>
                <b>
                    WIP Initial implementation of rollup_createBlock endpoint
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
        Created At 2022-07-19 12:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4132" class=".btn">#4132</a>
            </td>
            <td>
                <b>
                    Update RocksDB default block cache size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update RocksDB default block cache size to mitigate a performance regression from #3985.


Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We can see in the dashboard below that we have some blocks behind with the RocksDB block cache default value 8 MB, and Besu with block cache size 128 MB is performing better (no blocks behind).

<img width="1672" alt="image" src="https://user-images.githubusercontent.com/5099602/179716882-198371bf-97d5-4ed2-a725-6a802830f4ac.png">


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4128
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 09:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4131" class=".btn">#4131</a>
            </td>
            <td>
                <b>
                    Fix post merge chain reog with invalid block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

This PR fixes the failing Hive2 engine test `Invalid Ancestor Chain Re-Org, Invalid ReceiptsRoot, Invalid P8', Reveal using sync`

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 08:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4130" class=".btn">#4130</a>
            </td>
            <td>
                <b>
                    Useful response improves reputation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently there is no way for peers improve their reputation. With this PR peers improve their reputation when they send a useful response.

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 07:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4126" class=".btn">#4126</a>
            </td>
            <td>
                <b>
                    alternative malloc implementation - jemalloc
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
Use jemalloc with linux runtimes to better manage rocksdb memory usage.

* add malloc arena max envar to besu startup
* add jemalloc preload envar to besu startup
* add jemalloc lib download to docker jvm images

smoke tested and verified working on:
 Linux x86_64
 Docker linux aarch64 (on OSX M1)

Native OSX ([El Capitan +](https://developer.apple.com/forums/thread/13161https://developer.apple.com/forums/thread/13161)) is not loading jemalloc currently

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
potentially addresses:
#4057

## Documentation
If we end up going with jemalloc as an alternative malloc implementation for besu, we should document the need to have jemalloc installed in your environment, how to do it for each platform.

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 23:05:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4124" class=".btn">#4124</a>
            </td>
            <td>
                <b>
                    applies merge filtering to peers after 2 finalized
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
        Created At 2022-07-18 19:21:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4122" class=".btn">#4122</a>
            </td>
            <td>
                <b>
                    Check status of block propagation manager before starting or stopping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
In `DefaultSynchronizer` check if the `BlockPropagationManager` is running before starting or stopping it. This avoids an exception or warning if it is started or stopped more than once respectively.

## Fixed Issue(s)
fixes #4121

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 12:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4120" class=".btn">#4120</a>
            </td>
            <td>
                <b>
                    increase the default max message size for p2p messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current limit means that we are disconnecting useful peers during syncing.

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 06:01:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4118" class=".btn">#4118</a>
            </td>
            <td>
                <b>
                    EIP-1153: Transient storage opcodes
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

- Implement [EIP-1153: Transient storage opcodes](https://eips.ethereum.org/EIPS/eip-1153)
- Create new Shanghai spec for including this feature post Paris.
- Added a new `ByteCodeBuilder` class to make it easier to construct the E2E test cases.

## Eip1153 Tests 🆕

### TStoreEVMOperationTest.java
- [x]  load arbitrary value is 0 at beginning of transaction: `TLOAD(x)` is `0`
- [x]  loading after storing returns the stored value: `TSTORE(x, y)`, `TLOAD(x)` returns `y`
- [x]  loading any other slot after storing to a slot returns 0: `TSTORE(x, y)`, `TLOAD(x + n)` where `n > 0` returns `0`
- [x]  contracts have separate transient storage—loading a slot in a separate contract after storing returns 0: `TSTORE(x, y)`, `CALL(z, ...)`, `TLOAD(x)` returns `0`
- [x]  reentrant calls access the same transient storage: `TSTORE(x, y)`, `CALL(self, ...)`, `TLOAD(x)` returns `y`
- [x]  reentrant calls can manipulate the same transient storage: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `TLOAD(x)` returns `z`
- [x]  successfully returned calls do not revert transient storage writes: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `RETURN`, `TLOAD(x)` returns `z`
- [x]  revert undoes the transient storage write from the failed call: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `REVERT`, `TLOAD(x)` returns `y`
- [x]  revert undoes all the transient storage writes to the same key from the failed call, i.e. applies the modifications in reverse order: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `TSTORE(x, z + 1)` `REVERT`, `TLOAD(x)` returns `y`
- [x]  revert undoes transient storage writes from inner calls that successfully returned: `TSTORE(x, y)`, `CALL(self, ...)`, `CALL(self, ...)`, `TSTORE(x, y + 1)`, `RETURN`, `REVERT`, `TLOAD(x)` returns `y`
- [x]  delegatecall manipulates transient storage in the context of the current address: `TSTORE(x, y)`, `DELEGATECALL(a, ...)`, `TSTORE(x, z)`, `RETURN`, `TLOAD(x)` returns `z`
- [x]  delegatecall reads transient storage in the context of the current address: `TSTORE(x, y)`, `DELEGATECALL(a, ...)`, `TLOAD(x)` returns `y`
- [x]  transient storage cannot be manipulated in a static context: `TSTORE(x, y)`, `STATICCALL(a, ...)`, `TSTORE(x, z)` reverts
- [x]  transient storage cannot be manipulated in a static context when calling self: `TSTORE(x, y)`, `STATICCALL(self, ...)`, `TSTORE(x, z)` reverts
- [x]  transient storage cannot be manipulated in a nested static context: `TSTORE(x, y)`, `STATICCALL(self, ...)`, `CALL(self, ...)`, `TSTORE(x, z)` reverts
- [x]  Transient storage can be accessed in a static context when calling self`TSTORE(x, y)`, `STATICCALL(self, ...)`, `CALL(self, ...)`, `TLOAD(x)` returns `y`
- [ ] transient storage does not persist beyond a single transaction: TSTORE(x, y), RETURN, (new transaction to same contract), TLOAD(x, y) returns 0 

### TStoreOperationTest.java

- [x] Insufficient gas
- [x] Simple tstore test
- [x] TLoad uninitialized
- [x] TStore/TLoad 
- [x] TStore->TStore->TLoad
- [x] No gas refund

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

Unclear if I should add a new record to the changelog. Please advise.
- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-16 20:44:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4116" class=".btn">#4116</a>
            </td>
            <td>
                <b>
                    post-merge sync and peering fix 
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
addresses two sources of problems when syncing a post-merge network:

*  adds a merge-specific 'best peer' comparator rather than the PoW heaviest chain comparator.  This resolves a bug where besu would order its peers incorrectly and report that it did not have any peers with sufficient chain height: `No sync target with sufficient chain height, waiting for peers: {}`

* ensures 'fast' syncs (snap, checkpoint, fast) set the syncState as having reached TTD to satisfy preconditions for backward sync capability.  This fixes a 'stuck' issue where a fast sync would complete and catch up to a post-merge finalized block, but backward sync was not able to backfill from head back to the finalized block, and besu would just sit at its final fast sync pivot block.
 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3956
#3329

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-16 08:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4112" class=".btn">#4112</a>
            </td>
            <td>
                <b>
                    Update GraphQL to be closer to executioon-api spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Update GraphQL to be closer to execution-apis spec 

Update the graphQL to be closer to the execution-api specs.
This is a departure from EIP-1767 but the core devs have made it clear
that the execution-apis repo is considered canonical, not the EIP.

Major changes:
* Add support for EIP-2930 access lists
* Add support for EIP-1559 fees
* Add transaction, block, receipt, and header raw rlp fields
* Add chainID as base level query

Some items are still fake (fee estimate, effective tip).

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
        Created At 2022-07-15 00:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4107" class=".btn">#4107</a>
            </td>
            <td>
                <b>
                    [README] Add GitPOAP Badge to Display Number of Minted GitPOAPs for Contributors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Description**

Hey all, this PR adds a [GitPOAP Badge](https://docs.gitpoap.io/api#get-v1repoownernamebadge) to the README that displays the number of minted GitPOAPs for this repository by contributors to this repo.

You can see an example of this in [our Documentation repository](https://github.com/gitpoap/gitpoap-docs#gitpoap-docs).

This should help would-be contributors as well as existing contributors find out that they will/have received GitPOAPs for their contributions.

CC: @colfax23 @kayla-henrie


Signed-off-by: nixorokish

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add GitPOAP badge to README.md

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Add GitPOAP badge to README.md

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 17:40:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4106" class=".btn">#4106</a>
            </td>
            <td>
                <b>
                    Fix PR 4098
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

There was an error during the merge from main, that readded some deleted code, fixing it

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
        Created At 2022-07-14 16:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4105" class=".btn">#4105</a>
            </td>
            <td>
                <b>
                    Remove hash to append from the queue only if the step succeeds
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

In case of an error the first hash to fetch is lost, and then the backward sync tries to go ahead and start a forward sync.
Sample log 
[first-hash-not-retry.txt](https://github.com/hyperledger/besu/files/9112753/first-hash-not-retry.txt)

This PR remove the hash from the queue only when its successfully fetched

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
        Created At 2022-07-14 14:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4104" class=".btn">#4104</a>
            </td>
            <td>
                <b>
                    log execution errors at right level, stops transition message propagation post-merge sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log execution errors at right level, stops transition message propagation post-merge sync


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 13:40:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4103" class=".btn">#4103</a>
            </td>
            <td>
                <b>
                    Add experimental config option to enable v5 discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
Add experimental config option to enable v5 discovery## 

## Fixed Issue(s)
fixes #4088

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 12:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4102" class=".btn">#4102</a>
            </td>
            <td>
                <b>
                    Ignore 2 tests that assume that the system language is English, if that should not be the case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
2 of our tests that check error messages from the JVM assume that the system language is always English. If that is not the case, the JVM error messages will be localized and the tests will fail. This PR checks the system language before running those 2 tests and ignores them, if it is not English. If the system language is English the tests are executed like before.

## Fixed Issue(s)

fixes #2190

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 11:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4100" class=".btn">#4100</a>
            </td>
            <td>
                <b>
                    WIP Peer disco
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing a theory with EthPeer disconnects

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 03:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4099" class=".btn">#4099</a>
            </td>
            <td>
                <b>
                    Fix for RPC performance regression
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
PR #3695 uses [i.o.v.e.web.Route#blockingHandler](https://vertx.io/docs/apidocs/io/vertx/ext/web/Route.html#blockingHandler-io.vertx.core.Handler-) to attend JSON-RPC HTTP requests, but [according documentation](https://vertx.io/docs/vertx-web/java/#_using_blocking_handlers) it does it linearly. This PR adds `ordered=false` to let vert.x parallelize the processing.

## Fixed Issue(s)
fixes: #3959

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 20:26:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4098" class=".btn">#4098</a>
            </td>
            <td>
                <b>
                    Delegate all the block checks and validation to the block import phase
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

Remove preventive checks during sync, since they will be performed always performed during the import phase later, where the block will be also flagged as bad block.
With this the last failing Hive test (Invalid Ancestor Chain Re-Org, Invalid Number, Invalid P9', Reveal using sync) passes.

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
        Created At 2022-07-13 14:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4097" class=".btn">#4097</a>
            </td>
            <td>
                <b>
                    Finalised blocks should not prevent reorgs in BWS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We should allow reorgs bellow finalized blocks during Backwards Sync.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 14:00:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4096" class=".btn">#4096</a>
            </td>
            <td>
                <b>
                    Allow creating the Trie Log Layer objects outside of its package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small change to allow using the TrieLogLayer class outside its package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 13:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4095" class=".btn">#4095</a>
            </td>
            <td>
                <b>
                    Create backward sync retries on demand
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

Currently backward sync create the max number of retries ahead of time, and this could cause unneeded retries in case of non recoverable error like in this log 
[backward-sync-retries.txt](https://github.com/hyperledger/besu/files/9101478/backward-sync-retries.txt)

This PR rework the retry strategy to create retries on demand and fast fail in case of a non recoverable exception.


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
        Created At 2022-07-13 11:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4094" class=".btn">#4094</a>
            </td>
            <td>
                <b>
                    candidate fix for missing parent worldstate
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

when we remember block after the merge we must persist the trielog. because if we lose the trielog in the memory   (ex  restart besu) we can end up in a case where the block is saved but not the trielog. this can prevent the rollback or the rollforward to work because besu will consider that it can do it as the block is present but it will failed because trielog is missing. 

may be one of the reasons for the problem found on a ropsten test node

A possible edgecase description : 
- the head is block 5
- we remember block 6
- as we remember block 6 , we save trielog 6 only in memory
- CL is saying to go to block 7
now we have
- block5 in database + trielog 5 in database
- block6 in database + trielog 6 in memory
- block7 in database + trielog 7 in database
- we have a reorg to block 6
- we rollback 7 to 6 and we persist again block 6. as trielog 6 is not in the database we save invalid trielog 6 (7->6)

 if we restart before the reorg trielog 6 is missing
 
 this PR also fix an issue related to an invalid implementation of BonsaiInmemoryWorldstate
 
```java 
java.lang.AssertionError: Node hash 0x9289cda321472949c843ca0b1c6e08011c2608436898699468f49b72d2d8533e not equal to expected 0x03ac2557b39e96bc541432719417ca05360530f915ae8e53d8bf2591bee9c883
	at org.hyperledger.besu.ethereum.trie.StoredNodeFactory.lambda$retrieve$1(StoredNodeFactory.java:103)
	at java.base/java.util.Optional.map(Optional.java:265)
	at org.hyperledger.besu.ethereum.trie.StoredNodeFactory.retrieve(StoredNodeFactory.java:97)
	at org.hyperledger.besu.ethereum.trie.StoredNode.load(StoredNode.java:130)
	at org.hyperledger.besu.ethereum.trie.StoredNode.accept(StoredNode.java:63)
	at org.hyperledger.besu.ethereum.trie.StoredMerklePatriciaTrie.put(StoredMerklePatriciaTrie.java:142)
	at org.hyperledger.besu.ethereum.bonsai.BonsaiPersistedWorldState.calculateRootHash(BonsaiPersistedWorldState.java:227)
	at org.hyperledger.besu.ethereum.bonsai.BonsaiPersistedWorldState.calculateRootHash(BonsaiPersistedWorldState.java:104)
	at org.hyperledger.besu.ethereum.bonsai.BonsaiInMemoryWorldState.rootHash(BonsaiInMemoryWorldState.java:34)
	at org.hyperledger.besu.ethereum.MainnetBlockValidator.validateAndProcessBlock(MainnetBlockValidator.java:119)
	at org.hyperledger.besu.consensus.merge.blockcreation.MergeCoordinator.validateBlock(MergeCoordinator.java:256)
	at org.hyperledger.besu.consensus.merge.blockcreation.MergeCoordinator.rememberBlock(MergeCoordinator.java:272)
	at org.hyperledger.besu.consensus.merge.blockcreation.TransitionCoordinator.rememberBlock(TransitionCoordinator.java:137)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.engine.EngineNewPayload.syncResponse(EngineNewPayload.java:189)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.ExecutionEngineJsonRpcMethod.lambda$response$0(ExecutionEngineJsonRpcMethod.java:62)
	at io.vertx.core.impl.ContextImpl.lambda$null$0(ContextImpl.java:159)
	at io.vertx.core.impl.AbstractContext.dispatch(AbstractContext.java:100)
	at io.vertx.core.impl.ContextImpl.lambda$executeBlocking$1(ContextImpl.java:157)
	at io.vertx.core.impl.TaskQueue.run(TaskQueue.java:76)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
	at java.base/java.lang.Thread.run(Thread.java:829)
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4084
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 10:55:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4093" class=".btn">#4093</a>
            </td>
            <td>
                <b>
                    Revert "Add terminal block hash and number to Ropsten genesis file (#4026)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 27fc468624d4a19067b076567ea9e1578217d34e.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Reverting this commit since it is causing error in the CL clients and needs to be implemented in a different way

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
        Created At 2022-07-13 09:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4092" class=".btn">#4092</a>
            </td>
            <td>
                <b>
                    Backward sync exception improvements
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

During the investigation of a Hive test that triggers backward sync, found some improvements that could be applied to backward sync exceptions.

1) Remove of recoursive exceptions nesting, that produces monster exception like this one
[deeply-nested-exception.txt](https://github.com/hyperledger/besu/files/9100608/deeply-nested-exception.txt)

2) Avoid to return `null` from `syncBackwardsUntil` methods in case the block is already trusted

3) Log a warning for backward sync exception that are not recoverable, likewise it is already done for recoverable exceptions

4) Rephrase the error messages when there is a validator error found during the backward sync, with the assumption that the child block is the invalid one, and the parent is correct, this makes clearer the error message for the Hive test

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
        Created At 2022-07-13 09:07:37 +0000 UTC
    </div>
</div>

