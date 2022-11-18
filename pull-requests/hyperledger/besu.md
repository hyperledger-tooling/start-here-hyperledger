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
- Maybe Reduces acceptance tests duration by 15% (20 min to 17 min)

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
This PR introduces a new feature that allows besu to prune old chain data. Two experimental CLI options are introduced as well: `--Xchain-data-pruning-enabled` to turn on/off pruning and `--Xchain-data-pruning-blocks-retained` to specify the number of recent blocks to retain.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Linked to #4476 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4671" class=".btn">#4671</a>
            </td>
            <td>
                <b>
                    Port backward sync updates from 4655 and 4656 to 22.10.1-alpha
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
Porting from #4655 the update to the block import progess log to also include blocks imported during the final ProcessKnownAncestorsStep since that part could take some time if the backward sync was long.

Porting from #4656 adjustment to batch size and log fix

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
        Created At 2022-11-14 17:21:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4669" class=".btn">#4669</a>
            </td>
            <td>
                <b>
                    Some cleanup in Discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span>
            </td>
            <td>
                Some cleanup: The PeerBondedObserver was only ever used to call the connect() method on the RlpxAgent

Signed-off-by: Stefan <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 04:09:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4668" class=".btn">#4668</a>
            </td>
            <td>
                <b>
                    Remove misleading fastSyncEnabled variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description

- Rename fastSyncEnabled to fullSyncDisabled as it can mislead someone into the assumption that the sync mode is FAST SYNC while it may be snap/checkout.
- Pass SynchronizerConfiguration object down to EthProtocolManager instead of Boolean fastSyncEnabled

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-13 22:27:49 +0000 UTC
    </div>
</div>

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
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
When blocks execute and their worldstates are appended as trie logs, the blocks are not yet available in blockchain storage.  Blockheaders are required to create/roll a snapshot trie log to a particular state. This PR changes the SnapshotTrieLogManager to create mutable snapshots once  blocks are appended to the chain.

This fix:
* directly addresses a snapshot transaction memory leak, rather than relying on finalize() methods in #4645 
* should be more performant since mutable copies are correctly cached rather than created at request time
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
                <span class="chip">mainnet</span>
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
                <span class="chip">mainnet</span>
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

