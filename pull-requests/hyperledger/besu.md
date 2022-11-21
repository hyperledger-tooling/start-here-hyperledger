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
                PR <a href="https://github.com/hyperledger/besu/pull/4713" class=".btn">#4713</a>
            </td>
            <td>
                <b>
                    Add type field to eth_getTransactionReceipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description
Add type field to eth_getTransactionReceipt according to: https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_gettransactionreceipt

`type: DATA - integer of the transaction type, 0x00 for legacy transactions, 0x01 for access list types, 0x02 for dynamic fees.
`
## Fixed Issue(s)
fixes #4505

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

Needs to be updated:

besu-docs PR: 
https://github.com/hyperledger/besu-docs/pull/1205

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 04:55:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4712" class=".btn">#4712</a>
            </td>
            <td>
                <b>
                    Fix a bug that can cause the heal to be stuck during snapsync
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
        Created At 2022-11-20 22:53:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4711" class=".btn">#4711</a>
            </td>
            <td>
                <b>
                    Fix EOFv1 validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR changes EOF validation to check deployed code instead of _init code_

The values for testing were taken from tx [0x64d2b96](https://explorer.shandong.ethdevops.io/tx/0x64d2b9619141c93bf319a5c9b46bada38bc06e6825adfa7539c84f2878b19a53) of the Shandong testnet.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-20 12:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4710" class=".btn">#4710</a>
            </td>
            <td>
                <b>
                    Merge main into 22.10.x
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

merge main into 22.10.x ahead of burn-in over the weekend

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
        Created At 2022-11-18 23:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4709" class=".btn">#4709</a>
            </td>
            <td>
                <b>
                    Add post-run allocation output to EVMTool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Add a CLI flag --json-alloc that will output the post-execution state of the allocations the EVM Tool executed in. As well as post-execution state for state-tests.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->


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
        Created At 2022-11-18 20:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4708" class=".btn">#4708</a>
            </td>
            <td>
                <b>
                    Revert "make snapshots the default behavior"
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
In light of the stability fix for layered worldstates in #4700, and the higher performance of in-memory worldstates versus snapshot worldstates, this PR reverts the default behavior of bonsai back to layered worldstates:

This reverts commit 305897c075947ea73e71b0f5d68717163a3ea861.



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
        Created At 2022-11-18 18:38:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4706" class=".btn">#4706</a>
            </td>
            <td>
                <b>
                    Add checksum from junit-bom-5.9.0.module
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

Builds are failing due to missing checksum for `junit-bom-5.9.0.module`
https://app.circleci.com/pipelines/github/hyperledger/besu/18361/workflows/dcefad4b-3ba2-45b3-9ac0-03d39e063f29/jobs/111616/parallel-runs/0/steps/0-104

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
        Created At 2022-11-18 16:52:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4705" class=".btn">#4705</a>
            </td>
            <td>
                <b>
                    Remove log statements that are keeping references to objects for too long
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


Improvement in terms of reducing java heap used,
since the logs were keeping reference to blocks sent by newPayload, that causes high memory consumption during initial sync, and could be one of the causes that prevent to complete snap sync on low spec machines. Exceptions are also logged by the backward sync, so there is no loss of information.


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
        Created At 2022-11-18 16:08:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4704" class=".btn">#4704</a>
            </td>
            <td>
                <b>
                    add pruning during snapsync
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

The idea of this PR is to have a consistent and correct flat database after the snapsync in order to be able to use it during transactions and therefore no longer browse the tree. This will improve the performance of the SLOAD and Besu in general

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
        Created At 2022-11-18 10:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4703" class=".btn">#4703</a>
            </td>
            <td>
                <b>
                    Post Merge cleanup: remove latestValidAncestorDescendsFromTerminal
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

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 10:21:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4702" class=".btn">#4702</a>
            </td>
            <td>
                <b>
                    Update tessera image version to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description
Update tessera image version to latest 

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
        Created At 2022-11-18 08:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4701" class=".btn">#4701</a>
            </td>
            <td>
                <b>
                    Start privacyCluster non-bootnodes in parallel (acceptance test improvement)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description
Start non-bootnodes in parallel for privacy clusters (acceptance test only)
- may reduce some acceptance tests duration by 15%

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 07:26:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4700" class=".btn">#4700</a>
            </td>
            <td>
                <b>
                    Use snapshots for in-memory copies of layered worldstate
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

In `BonsaiLayeredWorldState.copy()`, use a snapshot worldstate as the basis for a BonsaiInMemoryWorldstate copy

Prevents stateroot mismatches that arise from the persisted worldstate being different than the worldstate assoicated with a given layered worldstate.

Also moves isolation test setup into an abstract class, and adds a new BonsaiInMemoryIsolationTest

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
        Created At 2022-11-18 06:11:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4697" class=".btn">#4697</a>
            </td>
            <td>
                <b>
                    Spike Spring Boot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                What if we would use a Spring Dependency Injection instead of our Builders?
What if we would only depend on mainnet parts of Besu project?

These and other questions might be answered in this PR. 

This is a first runabout and as such - It does not work yet. 
But it will...
Hopefully...

This PR creates a new subdirectory of besu where we depend on besu.
The Spring does not leak into besu code at the moment. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 15:42:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4694" class=".btn">#4694</a>
            </td>
            <td>
                <b>
                    Skip javadocs and sources checksum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Ignore javadocs and sources verification to avoid IDE errors

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
        Created At 2022-11-17 11:11:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4689" class=".btn">#4689</a>
            </td>
            <td>
                <b>
                    alpha - Restore updating chain head during backward sync
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

port #4688 to 22.10.1

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
        Created At 2022-11-16 15:48:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4688" class=".btn">#4688</a>
            </td>
            <td>
                <b>
                    Restore updating chain head during backward sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">syncing</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Updating chain head during backward sync was wrongly removed during the removal of the finalized block rule, this PR restore it and also complete the removal of the remaining dead code that was meant to manage the finalized rule., and some renaming to improve semantic.
Removed a log statement that was keeping reference to blocks sent by newPayload, that causes high memory consumption during initial sync.

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
        Created At 2022-11-16 12:41:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4687" class=".btn">#4687</a>
            </td>
            <td>
                <b>
                    WIP - default methods in Protocol Schedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is just a spike. This branch will get most probably abandoned in the future
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 10:02:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4686" class=".btn">#4686</a>
            </td>
            <td>
                <b>
                    Add chain data pruning experimental feature
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
This PR introduces a new feature that allows besu to prune old chain data. Three experimental CLI options are introduced as well: `--Xchain-data-pruning-enabled` to turn on/off pruning, `--Xchain-data-pruning-blocks-retained` to specify the number of recent blocks to retain and `--Xchain-data-pruning-frequency` to specify how often to perform chain data pruning.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Linked to #4476 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 04:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4682" class=".btn">#4682</a>
            </td>
            <td>
                <b>
                    Enable RocksDB bloomFilters
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
Enable RocksDB full bloom filters, with 10 bits per key.
The benefit from enabling Bloom filters is to improve read performance, more details [here](https://github.com/facebook/rocksdb/wiki/RocksDB-Bloom-Filter#usage-of-new-bloom-filter). I believe though this will work better if Besu is synced from the beginning with this configuration, because Bloom filters are created when new SST files are created.

Here are the results when we compare median (50th percentile) and 95th percentile values on newPayload calls.

<img width="1653" alt="Screenshot 2022-11-17 at 18 03 38" src="https://user-images.githubusercontent.com/5099602/202650039-f0218033-a0e9-4ea9-9287-bd107dfd1c0c.png">

We can see a [small overhead in CPU consumption](https://github.com/facebook/rocksdb/wiki/RocksDB-Bloom-Filter#usage-of-new-bloom-filter), but this doesn't affect block processing time as we still have a room for CPU usage.  

With Bloom Filters
<img width="1604" alt="image" src="https://user-images.githubusercontent.com/5099602/202651620-e8ac3c83-ef6f-4a22-939c-cc47d4396edc.png">

Without Bloom filters
<img width="1604" alt="Screenshot 2022-11-18 at 09 01 27" src="https://user-images.githubusercontent.com/5099602/202651805-676c17d7-b323-438a-ad94-989ce6342359.png">

Memory usage is quite similar, in the screenshot below we can see a little difference but not sure it is related to bloom filters

<img width="1604" alt="image" src="https://user-images.githubusercontent.com/5099602/202653316-db1e82da-3483-4554-99db-fea4b2d6d3c4.png">

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
        Created At 2022-11-15 15:10:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4680" class=".btn">#4680</a>
            </td>
            <td>
                <b>
                    Update Shandong genesis after Nov 5th restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
On Nov 5th the Shandong testnet was restarted due to a bug in the implementation of [EIP-3860](https://github.com/ethereumjs/ethereumjs-monorepo/pull/2397) in [ethereumjs](https://github.com/ethereumjs/ethereumjs-monorepo).

This PR makes the genesis for Shandong to match the hash of the current [running testnet](https://explorer.shandong.ethdevops.io/block/0) based on https://github.com/ethereumjs/consensus-deployment-ansible/blob/master/shandong-testnet/custom_config_data/genesis.json.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 12:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4679" class=".btn">#4679</a>
            </td>
            <td>
                <b>
                    Update artifact checksums after rebuilding the release
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 11:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4677" class=".btn">#4677</a>
            </td>
            <td>
                <b>
                    bugfix for 22.10.1 alpha
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
merge bugfix commit from #4648

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 08:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4676" class=".btn">#4676</a>
            </td>
            <td>
                <b>
                    Nightly CI step - reduce no output timeout for Quorum ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Occasionally these hang so we should not keep waiting for output

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 05:55:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4675" class=".btn">#4675</a>
            </td>
            <td>
                <b>
                    docker upload task - check for alpha and RC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Don't add `latest` tag if version ends in SNAPSHOT/alpha/beta/RC

Fixes #4674 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 01:26:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4673" class=".btn">#4673</a>
            </td>
            <td>
                <b>
                    22.10.1-alpha release - add SNAPSHOT to version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

add SNAPSHOT to version to avoid overwriting latest tags

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 22:12:39 +0000 UTC
    </div>
</div>

