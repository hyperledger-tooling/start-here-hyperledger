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
                PR <a href="https://github.com/hyperledger/besu/pull/4689" class=".btn">#4689</a>
            </td>
            <td>
                <b>
                    Restore updating chain head during backward sync
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

Updating chain head during backward sync was wrongly removed during the removal of the finalized block rule, this PR restore it and also complete the removal of the remaining dead code that was meant to manage the finalized rule., and some renaming to improve semantic

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
                <span class="chip">mainnet</span><span class="chip">logging</span>
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
{"@timestamp":"2022-11-14T13:52:25,896","level":"INFO","thread":"vert.x-worker-thread-0","class":"BackwardSyncContext","message":"Starting a new backward sync session","throwable":""}
{"@timestamp":"2022-11-14T13:52:26,177","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardsSyncAlgorithm","message":"Backward sync target block is 2288072 (0x5aa9afcbffaa4e337924bd73fed858321c41aec25267841566185b3e9e4cfaba)","throwable":""}
{"@timestamp":"2022-11-14T13:52:26,608","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2, 0.60% completed, downloaded 200 headers of at least 33147. Peers: 1","throwable":""}
{"@timestamp":"2022-11-14T13:52:36,644","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2, 42.84% completed, downloaded 14200 headers of at least 33147. Peers: 3","throwable":""}
{"@timestamp":"2022-11-14T13:52:46,712","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2, 94.13% completed, downloaded 31200 headers of at least 33147. Peers: 1","throwable":""}
{"@timestamp":"2022-11-14T13:52:47,861","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncStep","message":"Backward sync phase 1 of 2 completed, downloaded a total of 33200 headers. Peers: 1","throwable":""}
{"@timestamp":"2022-11-14T13:52:56,716","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 3.23% completed, imported 1070 blocks of at least 33156 (current head 2255995, target head 2288081). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:53:07,109","level":"INFO","thread":"nioEventLoopGroup-3-5","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 9.05% completed, imported 3001 blocks of at least 33157 (current head 2257926, target head 2288082). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:53:17,111","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 11.35% completed, imported 3764 blocks of at least 33158 (current head 2258689, target head 2288083). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:53:27,214","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 15.08% completed, imported 5001 blocks of at least 33158 (current head 2259926, target head 2288083). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:53:37,286","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 18.25% completed, imported 6050 blocks of at least 33158 (current head 2260975, target head 2288083). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:53:47,290","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 21.63% completed, imported 7173 blocks of at least 33159 (current head 2262098, target head 2288084). Peers: 3","throwable":""}
{"@timestamp":"2022-11-14T13:53:57,955","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 24.13% completed, imported 8001 blocks of at least 33160 (current head 2262926, target head 2288085). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:54:07,957","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 27.33% completed, imported 9062 blocks of at least 33161 (current head 2263987, target head 2288086). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:54:17,960","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 29.73% completed, imported 9860 blocks of at least 33162 (current head 2264785, target head 2288087). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:54:28,536","level":"INFO","thread":"nioEventLoopGroup-3-6","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 32.57% completed, imported 10801 blocks of at least 33163 (current head 2265726, target head 2288088). Peers: 2","throwable":""}
{"@timestamp":"2022-11-14T13:54:38,540","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 36.58% completed, imported 12133 blocks of at least 33164 (current head 2267058, target head 2288089). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:54:48,625","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 42.66% completed, imported 14149 blocks of at least 33164 (current head 2269074, target head 2288089). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:54:58,625","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 48.76% completed, imported 16171 blocks of at least 33164 (current head 2271096, target head 2288089). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:55:08,667","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 55.10% completed, imported 18275 blocks of at least 33164 (current head 2273200, target head 2288089). Peers: 3","throwable":""}
{"@timestamp":"2022-11-14T13:55:18,668","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 59.80% completed, imported 19832 blocks of at least 33165 (current head 2274757, target head 2288090). Peers: 3","throwable":""}
{"@timestamp":"2022-11-14T13:55:28,698","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 66.85% completed, imported 22170 blocks of at least 33166 (current head 2277095, target head 2288091). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:55:39,104","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 73.57% completed, imported 24401 blocks of at least 33167 (current head 2279326, target head 2288092). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:55:49,373","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 79.00% completed, imported 26201 blocks of at least 33167 (current head 2281126, target head 2288092). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:55:59,375","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 84.39% completed, imported 27991 blocks of at least 33167 (current head 2282916, target head 2288092). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:56:09,462","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 89.84% completed, imported 29797 blocks of at least 33168 (current head 2284722, target head 2288093). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:56:19,831","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 93.46% completed, imported 31001 blocks of at least 33169 (current head 2285926, target head 2288094). Peers: 5","throwable":""}
{"@timestamp":"2022-11-14T13:56:29,865","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 95.87% completed, imported 31801 blocks of at least 33170 (current head 2286726, target head 2288095). Peers: 7","throwable":""}
{"@timestamp":"2022-11-14T13:56:40,126","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2, 98.89% completed, imported 32801 blocks of at least 33170 (current head 2287726, target head 2288095). Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:56:42,603","level":"INFO","thread":"nioEventLoopGroup-3-7","class":"BackwardSyncContext","message":"Backward sync phase 2 of 2 completed, imported a total of 33170 blocks. Peers: 4","throwable":""}
{"@timestamp":"2022-11-14T13:56:42,612","level":"INFO","thread":"ForkJoinPool.commonPool-worker-3","class":"BackwardsSyncAlgorithm","message":"The Backward sync is done","throwable":""}
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
                <span class="chip">TeamChupa</span>
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
                <span class="chip">mainnet</span>
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
                <span class="chip">mainnet</span><span class="chip">TeamChupa</span>
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
                    Implement eth/67 sub protocol (EIP-4938)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
eth/67 ([EIP-4938](https://eips.ethereum.org/EIPS/eip-4938), March 2022)
Version 67 removed the GetNodeData and NodeData messages.

Besu:

- Supports multiple versions of a wire protocol.
- Does not break older clients, since they can keep using protocol version eth/66.
- For fast sync, eth/66 will be used

## Fixed Issue(s)
fixes #4596 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
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

